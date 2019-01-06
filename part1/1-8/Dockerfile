FROM java:8
WORKDIR /mydir

RUN apt-get -y update
RUN apt-get -y install git
RUN git clone https://github.com/nakkekakke/Calculator.git
WORKDIR /mydir/Calculator/src
RUN javac -cp . calculator/Calculator.java
CMD java -cp . calculator/Calculator
