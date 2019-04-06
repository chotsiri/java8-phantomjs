##Dev

###Build
    docker build -t java8-phantomjs:dev .


###Run
    docker run -it --name java8p java8-phantomjs:dev


##Prod
    docker tag java8-phantomjs:dev java8-phantomjs:1.0

##Push
    docker tag chotsiri/java8-phantomjs chotsiri/java8-phantomjs:1.0
    docker push chotsiri/java8-phantomjs:1.0
    
####Tag Dev
    docker tag chotsiri/java8-phantomjs:1.0 \
        docker01.dc2.true.th:5000/sbm/java8-phantomjs:1.0
        
####Tag MTG8
    docker tag java8-phantomjs:dev \
        mtg8-registry-01.true.th:5000/sbm/java8-phantomjs:1.0