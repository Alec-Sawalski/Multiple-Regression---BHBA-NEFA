# Multiple-Regression---BHBA-NEFA
## First Multiple Regression - BHBA
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + CE.Fat.Level + MS.Lactose + MS.Acetone.Log + MS.Urea + MS.pH + Cow.Breed + CE.Lame +                    BS.NEFA.0.7 + FPR.1.4 + (1 | CowID) Data: sub5_ncf_BHB

     AIC      BIC   logLik deviance df.resid 
     450.5    501.4   -213.2    426.5      502 

     Scaled residuals: 
    Min      1Q  Median      3Q     Max 
     -2.4340 -0.0409 -0.0154 -0.0010  9.0011 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 72.5     8.515   
     Number of obs: 514, groups:  CowID, 325

     Fixed effects:
               Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.4959     1.2075  -6.208 5.38e-10 ***
     MS.DIM           0.4782     0.3318   1.441   0.1495    
     CE.Fat.Level     0.1830     0.3928   0.466   0.6413    
     MS.Lactose      -0.5264     0.3793  -1.388   0.1652    
     MS.Acetone.Log   2.7647     0.5829   4.743 2.11e-06 ***
     MS.Urea          0.8043     0.4246   1.894   0.0582 .  
     MS.pH            0.7343     0.4849   1.514   0.1299    
     Cow.Breed02      2.7410     1.1801   2.323   0.0202 *  
     CE.Lame1        -0.7902     1.0990  -0.719   0.4721    
     BS.NEFA.0.71     0.3421     0.7559   0.453   0.6508    
     FPR.1.41         0.4604     0.7024   0.655   0.5122    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
          
     
 
