# Self Studies

## Brief

In this lesson, we will be learning about the concept of big data and data engineering. We will also explore one of the most popular NoSQL databases- MongoDB, and how to perform CRUD operations.

### Big Data

- [Introduction to Big Data](https://www.digitalocean.com/community/tutorials/an-introduction-to-big-data-concepts-and-terminology)


**Sofian's Notes**


1. Big data is a blanket term for the non-traditional strategies and technologies needed to gather, organize, process, and gather insights from large datasets.


2. Generally, big data is -
    
    a) large datasets i.e. too large to reasonably process or store with tradtional tools or on a single computer

    b) the category of computinf strategies and tech that are used to handle large datasets


3. In 2001, Gartner’s Doug Laney first presented what became known as the “three Vs of big data” to describe the <b><u>physical</u></b> characteristics that make big data different from other data processing:

    a) Volume

    b) Velocity (speed of information moving through the system, from multiple sources, with real-time processing)
        - real-time procesing implies transformation or changes to raw data will happen in memory during processing

    c) Variety (formats and type)

    d) Other Characteristics (<b><u>qualitative</u></b> characteristics):
        
        - Veracity (variety of data sources & complexity of processing)
        
        - Variability (wide variation in quality)
        
        - Value (costs of processing vs actual value)


4. The general categories of activities involved with big data processing are:
    
    a) Ingesting data into the system
        
        i) Apache Sqoop, Apache Flume, Apache Chukwa, <b><u>Apache Kafka</u></b>, Gobblin
        
        ii) ETL process - extract, transform and load (format, categorize and label)
    
    b) Persisting the data in storage
        
        i) <b><u>Apache Hadoop's</u></b> HDFS filesystem, Ceph, GlusterFS, NoSQL DB
    
    c) Computing and Analyzing data
        
        i) Apache Hadoop's <b><u>MapReduce</u></b> - Batch processing (larger chunks): Splitting > Mapping > Shuffling > Reducing > Assembling
        
        ii) Apache Storm, <b><u>Flink (fraud detection)</u></b> and <b><u>Spark</u></b> - Real-time or stream processing (smaller chunks)
    
    d) Visualizing the results
        
        i) Prometheus, Jupyter Notebook

    Clustered Computing - the foundation for technology used in each of the life cycle stages.
        
        i) Resource pooling e.g. available storage, CPU and RAM pooling
        
        ii) High Availability e.g. for real-time analytics
        
        iii) Easy Scalability e.g. for adding more machines to the group

        Software used - Hadoop's YARN (Yet Another Resource Negotiator)
                      - Apache Mesos



### JSON

Read up on JSON to understand the syntax and structure, as MongoDB stores data in a JSON-like format.

- [Introduction to JSON](https://www.digitalocean.com/community/tutorials/an-introduction-to-json)


**Sofian's Notes**


1. JSON, short for JavaScript Object Notation, is a format for sharing data


2. JSON is derived from the JavaScript programming language, but it’s available for use by many languages including Python, Ruby, PHP, and Java.


3. JSON uses the .json extension.

    a) A JSON object is a key-value data format that is typically rendered in curly brackets e.g.

        ```
        {
            "KEY" : "VALUE"
            "first_name" : "Sammy",
            "last_name" : "Shark",
            "location" : "Ocean",
            "online" : true,
            "followers" : 987 
        }
        ```
        # JSON values are on the left side of the colon, wrapped in double quptation marks.

            i) They need to be one of the following data-types e.g.

                - strings
                - numbers
                - objects
                - arrays
                - booleans
                - null

        ## JSON ignores white space but you are still encouraged to use underscores, e.g. first_name, to avoid issues in other languages.

    b) It can be defined in another file format e.g.html

    c) It can appear inside of quotes as a JSON string

    d) It can be an object assigned to a variable, transmitting between web server and client or browser


4) The most important attribute of JSON is that it can be readily transferred between programming languages in a format that all of the participating languages can work with. 
    
    - In contrast, JavaScript objects can only be worked with directly through the JavaScript programming language.


5) JSON can store nested objects in JSON format in addition to nested arrays, allowing you to work with more complicated and hierarchical data.