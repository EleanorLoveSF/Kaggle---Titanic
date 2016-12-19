##Inputting the Test and Train datasets into Rstudio
traindata<-read.csv("train.csv")
testData<-read.csv("test.csv")
head(traindata)

##Making basic visualizations in Rstudio
plot(density(traindata$Age,na.rm=TRUE))
plot(density(traindata$Fare,na.rm=TRUE))
plot(density(traindata$PassengerId,na.rm=TRUE))
plot(density(traindata$Survived,na.rm=TRUE))
plot(density(traindata$Fare,na.rm=TRUE))
#By first plotting the density we are able to get a sense of how the overall data feel and get a few bague answers:
#1.where is the general center?
#Is there a skew?
#Does is generally take higher values?
#Where are most of the values concentrated?

##Survival Rate by Sex Barplot
counts<-table(traindata$Survived,traindata$Sex)
barplot(counts,xlab = "Gender",ylab = "Number of People",main = "survived")
counts[2]/(counts[1]+counts[2])
counts[4]/(counts[3]+counts[4])
#74.2% of women survived versus 18.9% of men.

##Suvival Rate by Passaenger Class Barplot
Pclass_survival<-table(traindata$Survived,traindata$Pclass)
barplot(Pclass_survival,xlab="Cabin Class",ylab="Number of People",main="survived and deceased between male and female")
Pclass_survival[2]/(Pclass_survival[1]+Pclass_survival[2])
Pclass_survival[4]/(Pclass_survival[3]+Pclass_survival[4])
Pclass_survival[6]/(Pclass_survival[5]+Pclass_survival[6])
#63.0%, 1st class
#47.4%, 2nd class
#24.2%, 3rd class

##Conclusion
#The key idea is that we are trying to determine if any variables are realated to what we are trying to predict: Suvived.
