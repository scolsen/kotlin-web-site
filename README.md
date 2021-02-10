# Kotlin website
[![Official project][project-badge]][project-url]

This is the source for the [http://kotlinlang.org](http://kotlinlang.org).
     
<a id="project-structure"></a>
## Website structure 

### Content

|Source files|Location|Navigation|
|------------|--------|---------------|
|Kotlin docs |[docs/topics](docs/topics)| [kr.tree](docs/kr.tree)| 
|Community | [docs/pages/community](docs/pages/community) | [_nav.yml](data/_nav.yml) | 
|Education | [docs/pages/education](docs/pages/education)| [_nav.yml](data/_nav.yml)| 

Note that source files for KMM docs, coroutine docs, and language specification are stored in separate repositories:

* [kotlin-mobile-docs](https://github.com/JetBrains/kotlin-mobile-docs)
* [kotlinx.coroutines](https://github.com/Kotlin/kotlinx.coroutines/docs)
* [kotlin-spec](https://github.com/Kotlin/kotlin-spec)

The Kotlin grammar reference (grammar.xml) is generated by the [Kotlin grammar generator](https://github.com/JetBrains/kotlin-grammar-generator) from the
[Kotlin grammar definition](https://github.com/JetBrains/kotlin/tree/master/grammar).

### Configuration files

|Configuration| File|
|-----|----|
|Navigation and structure| [kr.tree](docs/kr.tree) for docs and [_nav.yml](data/_nav.yml) for other pages |
|Variables, such as release version | [v.list](docs/v.list) for docs and [releases.yml](data/releases.yml) for other pages |
|Community events on the map | [events.xml](data/events.xml) |
|Video list (outdated) | [videos.yml](data/videos.yml) |

### Templates

The Kotlin website uses [Jinja2](http://jinja.pocoo.org/docs/dev/) templates from the `templates` folder.
Note that all Markdown files, except for [docs](docs), are processed as Jinja templates before HTML conversion. 
This allows using all Jinja benefits for Markdown (for example, build URLs with the `url_for` function).


## Guidelines and markup

Follow [these Kotlin documentation guidelines on style and formatting](https://docs.google.com/document/d/1mUuxK4xwzs3jtDGoJ5_zwYLaSEl13g_SuhODdFuh2Dc/edit?usp=sharing).

For other pages, follow the complete syntax reference at the [kramdown site](http://kramdown.gettalong.org/syntax.html).
You can also include metadata fields. Learn more in the [Jekyll docs](http://jekyllrb.com/docs/frontmatter/).

## Local deployment

Currently, there is no way to deploy the Kotlin website locally. You can contribute to docs by sending us a pull request.

## Report issues

If you face an issue, report it to our issue tracker, [YouTrack](http://youtrack.jetbrains.com/issues/KT).

You can provide feedback on the revamped Kotlin documentation in this [YouTrack ticket](https://youtrack.jetbrains.com/issue/KT-44338).

[project-url]: https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub
[project-badge]: http://jb.gg/badges/official.svg
[slack-url]: http://slack.kotlinlang.org
