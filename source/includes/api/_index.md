# API Reference

The Cloudant API reference is intended to be a comprehensive and living catalog of Cloudant's capabilities. Contributions are welcome through [Cloudant Labs on GitHub](https://github.com/cloudant-labs/slate). The API reference content is built with [Slate](https://github.com/tripit/slate).

*For the cURL samples* There are three ways you can supply the username and password data for a request.
<br/>
1. The `-u $USERNAME` parameter on its own causes
cURL to ask you to enter your password interactively on the command line before performing the request. This option is used for the cURL examples in the Cloudant API reference.
<br/>
2. Entering the combination parameter `-u $USERNAME:$PASSWORD` as part of your command means that you are not asked to enter your password interactively.
However, a plain text copy of your password appears in the terminal log. This option is not secure.
<br/>
3. For an `https` cURL request, you can supply the username and password as part of the URL:
<br/>
`... https://$USERNAME:$PASSWORD@$USERNAME.cloudant.com ...`
<br/>
However, a plain text copy of your password appears in the terminal log. This option is not secure.

An alternative approach is to use a hashed version of your username and password combination and supply that data in your cURL command.
The Cloudant Blog article [Authorized curl, a.k.a acurl](https://cloudant.com/blog/authorized-curl-a-k-a-acurl) explains how to create
an `acurl` command that makes use of this technique, enabling you to enter
commands such as:
<br/>
`acurl https://$USERNAME.cloudant.com`
