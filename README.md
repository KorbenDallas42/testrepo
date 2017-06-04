# testrepo
# For week 5 class, profile in R


category = c("computer programming", "math", "statistics", "machine learning", "domain expertise", "communication and presentation skills", "visualization") 
ranking = c(4, 4, 3, 4, 1, 3, 2) 
profilet<-tibble(category, ranking)
profilet
profile = data.frame(category, ranking)   
colnames(profile)
profile

ggplot(data=profile, aes(x=category, y=ranking)) + geom_bar(stat="identity") +
  theme(axis.text.x = element_text(angle = 90, hjust = 1)) + 
  ggtitle("Data Science Profile")

