# spark-base-impl
A Basic/Template Implementation of Spark-Base

### Running locally
first, assemble fat jar with `sbt assembly`
then, you can submit a job like this    
```aidl
spark-submit \
--class in.tap.base.spark.impl.Main \
target/scala-2.11/spark-base-impl-assembly-1.0.0-SNAPSHOT.jar \
--step basic \
--in1 src/test/resources/basic/in/ \
--in1-format json \
--out1 src/test/resources/basic/out \
--out1-format json
```