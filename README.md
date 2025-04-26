

```{r }
waiting_time <- c(16,30,17,22,31,11,19,18,8)
t.test(waiting_time, mu = 15, alternative = "less",conf.level = 0.95)
```

##p-value is 0.9263 which is greater than 0.05 we accept the null that there is no evidence to support the waiting time is less than 15 minutes

```{r }
income <- c(12,16,20,15,14,8,11,17,13,7,10,6)
t.test(income, mu = 10, alternative = "two.sided",conf.level = 0.95)
```

## p-value is 0.0747 which is greater than 0.05 we accept the null that the CEO income is not different from 10

```{r }
blood_pressure <- c(183,178,152,157,194,163,144,114,179,150,118,158,165)
wilcox.test(blood_pressure, mu = 165, alternative = "less",exact = FALSE)
```

##p-value is 0.2163 which is greater than 0.05 we accept the null that the median blood pressure is equal to 165

```{r }
binom.test(2,12,p=0.4,conf.level = 0.90)
```

##since p-value is 0.1408 which is less than 0.4 we reject the null hypothesis at 10% significance and conclude that fewer than 40% of the injected drug users are HIV positive

##TWO INDEPENDENT SAMPLE TEST

```{r}
method1 <- c(1,14,19,12,11,15,20,5,21,15,15,28,3,6)
method2 <- c(16,17,19,10,31,22,26,24,27,32,14,8,12,11)
t.test(method1,method2, mu=0, alternative = "two.sided",conf.level = 0.95)
```

##p-value is 0.05071 which is greater than 0.05 hence we accept the null hypothesis that their is no difference between the two farming methods

```{r}
funci <- c(15,9,12,22,14,9,10,15)
malaria <- c(7,8,10,6,7,7,14,13,11,5)
t.test(funci,malaria, mu=0, alternative = "two.sided",conf.level = 0.95)
```

##p-value is 0.02991 which is less than 0.05 hence we reject the null hypothesis that their is no difference between the two effectiveness in treating malaria

```{r}
males <- c(2,3,5,6,4,2)
females <- c(5,9,8,10,7,6)
wilcox.test(males, females,exact = FALSE)
```

##the p-value is 0.01259 which is less than 0.05 hence we reject the null hypothesis that their is no difference in biomass
