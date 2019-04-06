##Dev

###Build
    docker build -t java8jre-phantomjs:dev .


###Run
    docker run -it --name java8p java8jre-phantomjs:dev


##Prod
    docker tag java8jre-phantomjs:dev java8jre-phantomjs:1.0

##Push
    docker push chotsiri/java8jre-phantomjs:1.0
    
####Tag Dev
    docker tag java8jre-phantomjs:dev \
        docker01.dc2.true.th:5000/sbm/java8jre-phantomjs:1.0
        
####Tag MTG8
    docker tag java8jre-phantomjs:dev \
        mtg8-registry-01.true.th:5000/sbm/java8jre-phantomjs:1.0