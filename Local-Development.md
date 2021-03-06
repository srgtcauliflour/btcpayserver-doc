# Local development

## Dependencies

If you want to help development you need:

* [.NET Core 2.0 SDK](https://microsoft.com/net/core/)
* Docker

## Which IDE?

I recommend using Visual Studio Code (cross platform) or Visual Studio 2017 update 3 (Windows Only).  
You can of course use VIM if you are hardcore, .NET Core 2.0 is command-line environment friendly.

## During development...

You need an instance of NBXplorer, Postgres, and Bitcoin Core running and configured on the right ports to execute tests and run the project for debugging.

To simplify the development process we created a docker-compose file which setup everything for your dev environment, you can find all the information in [the README of the test project](https://github.com/btcpayserver/btcpayserver/blob/master/BTCPayServer.Tests/README.md).

Both Visual Studio Code and Visual Studio 2017 will run the debug profile Docker-Regtest, which will run a BTCPay server instance connecting to the services in your docker service so you can easily debug and step through the code.  
