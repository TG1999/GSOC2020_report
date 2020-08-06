# GSoC 2019 project, Fetchcode

## Description

## Code

### Fetchcode:
1) Download reliably code from HTTP and FTP sources using a URL as input
2) Download reliably code from version control systems (VCS) such as git, hg, svn in a pluggable way.
3) Return information about a URL (possibly by making API calls). For instance, given a Git/GitHub/Gitlab/Bitbucket URL we should get details about the list of tags and versions. Or get details from a package using a PURL as an input by querying a package registry API.
Repository: https://github.com/nexb/fetchcode

My contributions: 


### PackageURL:

1) Be smart about URLs and provide ways to fix and resolve URLs. There is a basic feature in the Package URL Python library to get a PURL from a URL (See https://github.com/package-url/packageurl-python/blob/master/src/packageurl/contrib/url2purl.py ). This should be enhanced and furthered there and in ScanCode such that given a URL we can get a PURL, or given a Git/GitHub/Gitlab/Bitbucket URL we can get a normalized download URL.
2) Also able to convert URLs of type Github,Bitbucket and Gitlab to PURLs

Repository: https://github.com/package-url/packageurl-python/

Project link on pypa : https://pypi.org/project/packageurl-python/
