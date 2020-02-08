# Comandos HDFS


### Accediendo a HDFS

hdfs dfs put (local_path/archive.txt) (path_hdfs/archive.txt)

Spark: hdfs://nnhost:port/file..

### Manipulando archivos de HDFS

Leer: hdfs dfs -cat path_hdfs/archive.txt

Copiar a disco local: hdfs dfs -get (path_hdfs/archive.txt) (localfile.txt)

Borrando archivo: hdfs dfs -rm path_hdfs/file.txt

Borrando un conjunto de datos: hdfs dfs -rm (path_hdfs/*)

Borrando un directorio y su contenido hdfs dfs -rm -r (path_directory)

### Visualizar datos en HDFS

ver las primeras n lineas: hdfs dfs -cat (path_hdfs/archive.extension) | tail -n 5

Visualizar las primeras n lineas del archivo: hdfs dfs -cat (path_hdfs/archive.extension) | head -n 20


### Leer archivos Parquet

parquet-tools head archive.parquet

parquet-tools schema archive.parquet

### Leer archivos Avro

avro-tools tojson archive.avro

avro-tools getschema archive.avro

_Columnar organization avro vs parquet?_
