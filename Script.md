#load file
load(file.choose())

#load project file
setwd("F:/Gdrive/R")
load("Project1.Rdata")

#Laptop
setwd("E:/Google drive/R")
load("Project1.Rdata")

#save
save.image(file.choose())

#attach file
attach(data)

#Gender
class(Gender)
mean(Age)
rm(list = ls())

#install ePiR
install.packages("epiR")

#remove package
remove.packages("epiR")

#bar plot percentage with labels
barplot(percentgender, main = "Gender distribution ", xlab = "Gender", ylab = "%", las=1 )
#horizontal plot
barplot(percentgender, main = "Gender Distribution", xlab= "Gender", ylab= "Percentage", las=1, horiz = T)
#pie chart
pie(count, main= "Gender")

#femdata
summary(femdata)
