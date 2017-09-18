# argument-bioconll-export-example
Example how to export labeled arguments to BIO CoNLL format. Based on the stable 0.1.0 version of DKPro-Argumentation that is available on Maven central.

Download and unzip the annotated corpus here:

https://www.ukp.tu-darmstadt.de/data/argumentation-mining/argument-annotated-user-generated-web-discourse/

Compile the project

```
$ mvn package
```

Run it with two parameters: input path (the unzipped data) and output path

```
$ java -cp target/lib/*:target/argument-bioconll-export-example-1.0-SNAPSHOT \
.jar com.github.habernal.ArgumentationCorpusBIOTokenExporter \
 habernal.gurevych.2015.argumentation.mining.CL.data/data/gold.data.toulmin/ /tmp/output-dir
```
