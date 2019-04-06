##Dev
###Build
    docker build -t java8jre-phantomjs:dev .
###Run
    docker run -it --name java8p java8jre-phantomjs:dev
    
##Prod
    docker tag java8jre-phantomjs:dev java8jre-phantomjs:1.0