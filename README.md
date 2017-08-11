# menagerie
Index package for all my random Python libraries

Apologies for the strange names, they all come from either 30 seconds of searching wikipedia for something that seems fitting, or failing that, looking around my house and grabbing random proper nouns.

## sunyata - Tools for publishing a serverless website/API.

[Sunyata](https://github.com/stevenorum/sunyata) (named after [a Buddhist concept of nothingness](https://en.wikipedia.org/wiki/Śūnyatā)) is a tool to publish simple APIs and websites using Lambda and API Gateway.

## junko - Framework for building a serverless website/API.

[Junko](https://github.com/stevenorum/junko) (named after [my cat Junko](https://github.com/stevenorum/menagerie/raw/master/files/junko.png), who is herself named after [Junko Tabei](https://en.wikipedia.org/wiki/Junko_Tabei) because she's always climbing stuff) is a bunch of helper stuff to make it as simple as possible to spin up a basic website with sunyata.  For an example, see [junko-example](https://github.com/stevenorum/junko-example).

## tenzing and tenzing-repo - Serverless dynamic pip repo.

[Tenzing](https://github.com/stevenorum/tenzing) and [tenzing-repo](https://github.com/stevenorum/tenzing-repo) (named after [my cat Tenzing](https://github.com/stevenorum/menagerie/raw/master/files/tenzing.png), who is himself named after [Tenzing Norgay](https://en.wikipedia.org/wiki/Tenzing_Norgay) because he's also always climbing stuff) are a pip repo based on Lambda and S3, and tools for uploading packages to those repos.  I wrote it because I didn't have a good way to install these random packages I write.  I don't feel like pushing them out to the public pip repo, as they're largely janky, untested, and not designed for general use, but I still wanted a way to install them in a mostly-normal fashion.  It also supports basic auth, and the URLs it uses to vend packages are short-lived presigned URLs, so it's at least slightly secure for keeping private stuff private.

## random disclaimers

Note: All of these tools that deal with cloud services are designed for use with AWS and AWS only, as they were initially developed for specific stuff I wanted to build and I do all my cloud development using AWS.  At this time I have no plans to add support for other ecosystems.

Note 2: Although I generally attempt to write secure software, none of the packages here have had any sort of in-depth security review or pen test.  I make no claims as to their security, even the ones that attempt to have a bit like tenzing-repo with auth enabled.
