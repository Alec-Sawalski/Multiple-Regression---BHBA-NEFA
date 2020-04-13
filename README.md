# Multiple-Regression---BHBA-NEFA

## BHBA Multiple Regression

#### Below is our first model of multiple regression with all significant predictors associated with BHBA. After running this first model, we used backward step elimination, eliminating the least significant predictor and re-running the model. 

#### BHBA Multiple Regression - First Model
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + CE.Fat.Level + MS.Lactose + MS.Acetone.Log 
     + MS.Urea + MS.pH + Cow.Breed + CE.Lame + 
     BS.NEFA.0.7 + FPR.1.4 + (1 | CowID) 
     Data: sub5_ncf_BHB

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
     
#### BHBA Multiple Regression - Final Model
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.Acetone.Log + Cow.Breed + (1 | CowID)
     Data: sub5_ncf_BHB

       AIC      BIC   logLik deviance df.resid 
     455.8    472.8   -223.9    447.8      517 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -2.2490 -0.0442 -0.0176 -0.0010  6.0287 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 73.23    8.558   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
                   Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.4096     1.1279  -6.569 5.05e-11 ***
     MS.Acetone.Log   2.7440     0.5014   5.472 4.45e-08 ***
     Cow.Breed02      2.9418     1.1095   2.651  0.00801 ** 
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### After the addition of Fatty Acids, we found that no Fatty Acids were significant predictors. Therefore, our final model was determined without the addition of Fatty Acids. 

## BHBA Odds Ratio's, Confidence Intervals, and Effect Plots

                         OR        2.5 %       97.5 %
     (Intercept)    1.554846e+01 6.289893e-05 6.431509e-03
     MS.Acetone.Log 1.894910e+01 6.394550e+00 4.633322e+01
     Cow.Breed02    6.054013e-04 2.177258e+00 1.928642e+02
 
<img src=https://user-images.githubusercontent.com/61294969/79125835-6ef56900-7d64-11ea-8772-8b28c2535158.png>

## NEFA Multiple Regression

#### Below is our first model of multiple regression with all significant predictors associated with NEFA. After running this first model, we used backward step elimination, eliminating the least significant predictor and re-running the model. 

#### NEFA Multiple Regression - First Model
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +  
     CE.Fat.Level + MS.pH + Cow.Breed + BS.Month_warm + CE.Stom.Layering +      
     BS.BHBA.1.2 + CE.Lame + (1 | CowID:Farm.No)
     Data: sub4nc_FA

     AIC      BIC   logLik deviance df.resid 
     481.4    536.5   -227.7    455.4      499 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -3.0227 -0.3775 -0.2382  0.2557  6.2066 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.656    1.287   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                      Estimate Std. Error z value Pr(>|z|)    
     (Intercept)           -1.10638    0.72661  -1.523  0.12784    
     BS.MS.Date.Difference -0.18253    0.15177  -1.203  0.22910    
     MS.DIM                -0.23846    0.15037  -1.586  0.11278    
     FPR.1.41               0.97354    0.31976   3.045  0.00233 ** 
     MS.Acetone.Log         0.80585    0.21261   3.790  0.00015 ***
     CE.Fat.Level           0.47353    0.16756   2.826  0.00471 ** 
     MS.pH                  0.01278    0.15331   0.083  0.93356    
     Cow.Breed02           -0.52252    0.44761  -1.167  0.24307    
     BS.Month_warm1         0.24806    0.31733   0.782  0.43438    
     CE.Stom.Layering1     -1.43661    0.72308  -1.987  0.04695 *  
     BS.BHBA.1.21           0.39613    0.36784   1.077  0.28153    
     CE.Lame1               0.44875    0.42605   1.053  0.29221    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Final Model
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ FPR.1.4 + MS.Acetone.Log + CE.Fat.Level + (1 |CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     476.8    498.0   -233.4    466.8      509 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -2.6028 -0.3849 -0.2465  0.2621  5.4450 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.764    1.328   
     Number of obs: 514, groups:  CowID:Farm.No, 325

     Fixed effects:
                    Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -2.3067     0.3324  -6.939 3.96e-12 ***
     FPR.1.41         0.9202     0.3060   3.007  0.00264 ** 
     MS.Acetone.Log   1.0369     0.2022   5.129 2.92e-07 ***
     CE.Fat.Level     0.5509     0.1648   3.342  0.00083 ***
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

## NEFA Multiple Regression - Addition of Fatty Acid

#### After finding a final model without the addition of fatty acids with NEFA, we added in individual fatty acids to the model and included the fatty acid that produced the best fit, which was Oleic acid. After the addition of Oleic acid, we once again did backward step elimination.

#### NEFA Multiple Regression - First Model with Fatty Acid
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ FPR.1.4 + MS.Acetone.Log + CE.Fat.Level + MS.Oleic +      (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     371.5    395.2   -179.7    359.5      379 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -3.9578 -0.3920 -0.2446  0.3269  2.4875 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.713    1.309   
     Number of obs: 385, groups:  CowID:Farm.No, 236

     Fixed effects:
                    Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -1.4907     0.3524  -4.230 2.34e-05 ***
     FPR.1.41        -0.5320     0.4750  -1.120 0.262715    
     MS.Acetone.Log   0.3415     0.2569   1.329 0.183761    
     CE.Fat.Level     0.3785     0.1842   2.054 0.039930 *  
     MS.Oleic         1.3971     0.3634   3.844 0.000121 ***
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Final Model with Fatty Acid
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ MS.Acetone.Log + CE.Fat.Level + MS.Oleic + (1 |CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     370.8    390.5   -180.4    360.8      380 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -3.2997 -0.4031 -0.2443  0.3630  2.5982 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.635    1.279   
     Number of obs: 385, groups:  CowID:Farm.No, 236

     Fixed effects:
               Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -1.7137     0.3056  -5.608 2.04e-08 ***
     MS.Acetone.Log   0.3827     0.2509   1.525   0.1272    
     CE.Fat.Level     0.3917     0.1822   2.149   0.0316 *  
     MS.Oleic         1.1521     0.2719   4.237 2.26e-05 ***
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

## NEFA Odds Ratio's, Confidence Intervals, and Effect Plots
                         OR      2.5 %     97.5 %
     (Intercept)    1.4661651 0.07943635  0.2954894
     MS.Acetone.Log 1.4795185 0.90416028  2.4831767
     CE.Fat.Level   3.1647980 1.04739544  2.1979837
     MS.Oleic       0.1801901 1.96843685  6.0445656

<img src=https://user-images.githubusercontent.com/61294969/79128874-d6fa7e00-7d69-11ea-8eb9-b886f97834d3.png>
