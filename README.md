# Hierarchical-linear-regression

```{r}
model1 <- lmer(formula =Total_agg_ST ~ 1 +	
               
               Age +	Parents_checking +	Parent_concern_need + Sibling +	Car_status + Financial_aids +	Grant	+ Scholarship	+ Loan + Major_of_study +	Time_Academic +	Time_Extracurricular +	Time_work +	Time_social +	Time_family +	 Co_op +	Internship +	GPA +	Ethinicity_1	+  Gender_1 +Father_education_1	+ Mother_education_1	+ Houshold_status_1+ Houshold_living_status_1 +
               (1|Participants_ID_all),
               
               
               data    = Milad325_7)

summary(model1)
    require(lmerTest)
coef(model1)
  AIC(model1)
```

```{r}
model2 <- lmer(formula =Total_agg_ST ~ 1 +	
               
               Age +	Parents_checking +	Parent_concern_need + Sibling +	Car_status + Financial_aids +	Grant	+ Scholarship	+ Loan + Major_of_study +	Time_Academic +	Time_Extracurricular +	Time_work +	Time_social +	Time_family +	 Co_op +	Internship +	GPA +	Ethinicity_1	+  Gender_1 +Father_education_1	+ Mother_education_1	+ Houshold_status_1+ Houshold_living_status_1 +
               (1|Participants_ID_all_minus_1),
               
               
               data    = Milad325_7)

summary(model2)
    require(lmerTest)
coef(model2)
  AIC(model2)
```

