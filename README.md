# beam-go by Rohit Chandupatla

### All of these commands should be run in Powershell.

## Set up your environment

The Beam SDK for Go requires go version **1.16 or newer**. It can be downloaded **[here](https://go.dev/)**. Check that you have version 1.16 by running:

```
go version
```

Once you've double-checked that you have the latest **version** of Go

```
go mod init github.com/rohitchandupatla/beam-go
```

To open **VS Code** in your local environment,
```
code .
```

Create the sample **[hello.go](https://raw.githubusercontent.com/RohitChandupatla/beam-go/main/hello.go)** file

When done, now use
```
go run .
```

After my **hello.go** has worked in your system, it's time to test my code locally.

Create **sample.txt** with Shakespeare content from **[here](https://raw.githubusercontent.com/RohitChandupatla/beam-go/main/sample.txt)**.

## Get the SDK and the examples

The easiest way to obtain the Apache Beam Go SDK is via **go get**:
```
go get -u github.com/apache/beam/sdks/v2/go/pkg/beam
```
### Run wordcount

The Apache Beam examples directory has many examples. All examples can be run by passing the required arguments described in the examples.

to **run** wordcount, run:
```
go install github.com/apache/beam/sdks/v2/go/examples/wordcount
```
To get the **output**, you must now run this command.
```
wordcount --input sample.txt --output rohitoutput
```

If you get my code, great; if not, try these commands because they work in a few local systems but not in mine, so I'm providing **additional commands** to run my code.

```
go get github.com/apache/beam/sdks/v2/go/pkg/beam/io/filesystem/gcs@v2.37.0
```

Now is the time to **build** in your local environment, so use these commands.

```
go build hello.go
```
```
go build wordcount.go
```

Now it's time to get the **output**. You'll be able to see my outcomes now.
```
.\hello.go
```
```
.\wordcount --input sample.txt --output rohitoutput
```
```
Get-Content rohitoutput
```

Now you can see my output locally, and I've also added it to my repo **[here](https://github.com/RohitChandupatla/beam-go/blob/main/rohitoutput).**
