# Google Summer of Code 2020 Final Report
## Organization - [Aboutcode](https://www.aboutcode.org/)
### Project -Fetchcode: A smart Code downloader
[Fetchcode](https://github.com/nexB/fetchcode)
1) Download reliably code from HTTP and FTP sources using a URL as input
2) Download reliably code from version control systems (VCS) such as git, hg, svn in a pluggable way.
3) Return information about a URL (possibly by making API calls). For instance, given a GitHub/Bitbucket/Npm/Pypi/Cargo/Rubygems URL we should get details about the list of tags and versions. Or get details from a package using a PURL as an input by querying a package registry API.

My contributions: 

| PR       | Status             | Description          |
|-----------------------|-------------------|---------------------|
| [#22](https://github.com/nexB/fetchcode/pull/22) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support for downloading http and ftp urls |
| [#30](https://github.com/nexB/fetchcode/pull/30) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add VCS Support |
| [#31](https://github.com/nexB/fetchcode/pull/31) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support for git URLs |
| [#39](https://github.com/nexB/fetchcode/pull/39) | ![Open](https://i.imgur.com/Mjp2nr7.jpg) | Add package registry support |

### PackageURL:

1) Be smart about URLs and provide ways to fix and resolve URLs. There is a basic feature in the Package URL Python library to get a PURL from a URL (See https://github.com/package-url/packageurl-python/blob/master/src/packageurl/contrib/url2purl.py ). This should be enhanced and furthered there and in ScanCode such that given a URL we can get a PURL, or given a Git/GitHub/Gitlab/Bitbucket URL we can get a normalized download URL.
2) Also able to convert URLs of type Github,Bitbucket and Gitlab to PURLs

My contributions: 

| PR       | Status             | Description          |
|-----------------------|-------------------|---------------------|
| [#39](https://github.com/package-url/packageurl-python/pull/39) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support converting PURLs to URLs |
| [#34](https://github.com/package-url/packageurl-python/pull/34) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support for github and BitBucket URLs  |

Repository: https://github.com/package-url/packageurl-python/

Project link on pypa : https://pypi.org/project/packageurl-python/

### Pre GSOC

| PR       | Status             | Description          |
|-----------------------|-------------------|---------------------|
| [#24](https://github.com/package-url/packageurl-python/pull/24) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support for rust packages |
| [#41](https://github.com/package-url/packageurl-python/pull/41) | ![Merged](https://i.imgur.com/YnDnRzm.jpg) | Add support for hackage PURLs  |


I want to thank Google and Aboutcode for giving me this opportunity to work with such an amazing community. I am blessed to have mentors ([Philippe Ombredanne](https://github.com/pombredanne) and [Steven Esser](https://github.com/majurg)) for helping me throughout the summer and help me to learn how to write production level code!
