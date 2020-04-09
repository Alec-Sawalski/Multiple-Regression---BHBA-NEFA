# Multiple-Regression---BHBA-NEFA

## BHBA Multiple Regression

#### BHBA Multiple Regression - Step 1
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
          
          
#### BHBA Multiple Regression - Step 2
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + MS.Lactose + MS.Acetone.Log + MS.Urea +     
     MS.pH + Cow.Breed + CE.Lame + FPR.1.4 + (1 | CowID)
     Data: sub5_ncf_BHB

     AIC      BIC   logLik deviance df.resid 
     455.7    498.2   -217.8    435.7      511 

     Scaled residuals: 
    Min      1Q  Median      3Q     Max 
    -2.5294 -0.0404 -0.0145 -0.0006 10.5500 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 76.29    8.734   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
                    Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.4601     1.1740  -6.354 2.09e-10 ***
     MS.DIM           0.4702     0.3192   1.473   0.1408    
     MS.Lactose      -0.4953     0.3737  -1.325   0.1851    
     MS.Acetone.Log   2.9548     0.5749   5.139 2.76e-07 ***
     MS.Urea          0.8471     0.4267   1.985   0.0471 *  
     MS.pH            0.7548     0.4814   1.568   0.1169    
     Cow.Breed02      2.7009     1.1948   2.261   0.0238 *  
     CE.Lame1        -0.8157     1.1017  -0.740   0.4590    
     FPR.1.41         0.4224     0.7029   0.601   0.5479    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### BHBA Multiple Regression - Step 3
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + MS.Lactose + MS.Acetone.Log + MS.Urea +     
     MS.pH + Cow.Breed + CE.Lame + (1 | CowID)
     Data: sub5_ncf_BHB

     AIC      BIC   logLik deviance df.resid 
     454.0    492.3   -218.0    436.0      512 

     Scaled residuals: 
    Min      1Q  Median      3Q     Max 
     -2.5681 -0.0384 -0.0140 -0.0006 11.3772 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 79.78    8.932   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
               Estimate Std.     Error    z value Pr(>|z|)    
     (Intercept)     -7.3973     1.1334  -6.527 6.72e-11 ***
     MS.DIM           0.4954     0.3168   1.564   0.1179    
     MS.Lactose      -0.5162     0.3789  -1.362   0.1731    
     MS.Acetone.Log   3.0241     0.5675   5.329 9.87e-08 ***
     MS.Urea          0.8877     0.4218   2.105   0.0353 *  
     MS.pH            0.7668     0.4769   1.608   0.1079    
     Cow.Breed02      2.7576     1.2096   2.280   0.0226 *  
     CE.Lame1        -0.7194     1.0839  -0.664   0.5069    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### BHBA Multiple Regression - Step 4
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + MS.Lactose + MS.Acetone.Log + MS.Urea +      
     MS.pH + Cow.Breed + (1 | CowID)
     Data: sub5_ncf_BHB

     AIC      BIC   logLik deviance df.resid 
     452.5    486.6   -218.3    436.5      513 

     Scaled residuals: 
    Min      1Q  Median      3Q     Max 
     -2.5836 -0.0398 -0.0151 -0.0007 10.8939 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 75.13    8.668   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
                     Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.3625     1.1494  -6.406  1.5e-10 ***
     MS.DIM           0.4802     0.3111   1.544   0.1227    
     MS.Lactose      -0.5294     0.3767  -1.405   0.1599    
     MS.Acetone.Log   2.9996     0.5589   5.367  8.0e-08 ***
     MS.Urea          0.8786     0.4178   2.103   0.0355 *  
     MS.pH            0.8123     0.4648   1.748   0.0805 .  
     Cow.Breed02      2.8206     1.1934   2.363   0.0181 *  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
#### BHBA Multiple Regression - Step 5
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.DIM + MS.Acetone.Log + MS.Urea + MS.pH + Cow.Breed +      
     (1 | CowID)
     Data: sub5_ncf_BHB

     AIC      BIC   logLik deviance df.resid 
     452.6    482.4   -219.3    438.6      514 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
    -2.5515 -0.0399 -0.0144 -0.0008 11.7415 
     
     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 74.94    8.657   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
                    Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.4434     1.1405  -6.526 6.74e-11 ***
     MS.DIM           0.3786     0.2973   1.274  0.20279    
     MS.Acetone.Log   3.0214     0.5611   5.384 7.27e-08 ***
     MS.Urea          0.8843     0.4191   2.110  0.03485 *  
     MS.pH            0.5839     0.3971   1.470  0.14146    
     Cow.Breed02      3.0719     1.1759   2.612  0.00899 ** 
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1
     
#### BHBA Multiple Regression - Step 6
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.Acetone.Log + MS.Urea + MS.pH + Cow.Breed +      
     (1 | CowID)
     Data: sub5_ncf_BHB

      AIC      BIC   logLik deviance df.resid 
     452.2    477.7   -220.1    440.2      515 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -2.4219 -0.0415 -0.0152 -0.0007  8.9072 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 73.65    8.582   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
               Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.4214     1.1737  -6.323 2.57e-10 ***
     MS.Acetone.Log   2.9307     0.5544   5.287 1.25e-07 ***
     MS.Urea          0.7973     0.4165   1.914   0.0556 .  
     MS.pH            0.7061     0.4266   1.655   0.0979 .  
     Cow.Breed02      3.0216     1.1735   2.575   0.0100 *  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### BHBA Multiple Regression - Step 7
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.BHBA.1.2 ~ MS.Acetone.Log + MS.Urea + Cow.Breed + (1 | CowID)
     Data: sub5_ncf_BHB

       AIC      BIC   logLik deviance df.resid 
      453.9    475.2   -222.0    443.9      516 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -2.2708 -0.0468 -0.0186 -0.0013  7.0573 

     Random effects:
     Groups Name        Variance Std.Dev.
     CowID  (Intercept) 65.01    8.063   
     Number of obs: 521, groups:  CowID, 328

     Fixed effects:
                   Estimate Std. Error z value Pr(>|z|)    
     (Intercept)     -7.0702     1.1337  -6.236 4.48e-10 ***
     MS.Acetone.Log   2.6370     0.4959   5.317 1.05e-07 ***
     MS.Urea          0.7466     0.3848   1.940   0.0524 .  
     Cow.Breed02      2.6846     1.0889   2.466   0.0137 *  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### BHBA Multiple Regression - Step 8
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

## BHBA Odds Ratio's, Confidence Intervals, and Effect Plots

## NEFA Multiple Regression

#### NEFA Multiple Regression - Step 1
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

#### NEFA Multiple Regression - Step 2
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +  
     CE.Fat.Level + Cow.Breed + BS.Month_warm + CE.Stom.Layering +      
     BS.BHBA.1.2 + CE.Lame + (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     479.4    530.3   -227.7    455.4      500 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -3.0205 -0.3786 -0.2382  0.2552  6.1993 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.654    1.286   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                           Estimate Std. Error z value Pr(>|z|)    
     (Intercept)            -1.1083     0.7258  -1.527 0.126783    
     BS.MS.Date.Difference  -0.1829     0.1517  -1.206 0.227805    
     MS.DIM                 -0.2365     0.1485  -1.593 0.111123    
     FPR.1.41                0.9744     0.3195   3.050 0.002290 ** 
     MS.Acetone.Log          0.8030     0.2095   3.833 0.000127 ***
     CE.Fat.Level            0.4735     0.1675   2.826 0.004712 ** 
     Cow.Breed02            -0.5254     0.4462  -1.177 0.239034    
     BS.Month_warm1          0.2483     0.3172   0.783 0.433770    
     CE.Stom.Layering1      -1.4340     0.7220  -1.986 0.047006 *  
     BS.BHBA.1.21            0.3970     0.3676   1.080 0.280246    
     CE.Lame1                0.4418     0.4179   1.057 0.290338    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 3
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +      
     CE.Fat.Level + Cow.Breed + CE.Stom.Layering + BS.BHBA.1.2 +  
     CE.Lame + (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     478.1    524.7   -228.0    456.1      501 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -3.1916 -0.3732 -0.2360  0.2416  5.9520 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.652    1.285   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                           Estimate Std. Error z value Pr(>|z|)    
     (Intercept)            -1.0183     0.7128  -1.429  0.15311    
     BS.MS.Date.Difference  -0.1819     0.1517  -1.199  0.23054    
     MS.DIM                 -0.2368     0.1485  -1.595  0.11074    
     FPR.1.41                0.9390     0.3154   2.978  0.00290 ** 
     MS.Acetone.Log          0.8237     0.2088   3.945 7.97e-05 ***
     CE.Fat.Level            0.4896     0.1669   2.933  0.00336 ** 
     Cow.Breed02            -0.4783     0.4408  -1.085  0.27790    
     CE.Stom.Layering1      -1.4048     0.7180  -1.957  0.05038 .  
     BS.BHBA.1.21            0.3993     0.3674   1.087  0.27711    
     CE.Lame1                0.4754     0.4148   1.146  0.25172    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 4
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +      
     CE.Fat.Level + CE.Stom.Layering + BS.BHBA.1.2 + CE.Lame +  
     (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     477.3    519.7   -228.6    457.3      502 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -3.2297 -0.3672 -0.2373  0.2410  5.3762 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.668    1.291   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                      Estimate Std. Error z value Pr(>|z|)    
     (Intercept)            -1.0775     0.7168  -1.503  0.13280    
     BS.MS.Date.Difference  -0.1915     0.1515  -1.264  0.20628    
     MS.DIM                 -0.2303     0.1480  -1.556  0.11969    
     FPR.1.41                0.9006     0.3123   2.884  0.00393 ** 
     MS.Acetone.Log          0.8719     0.2071   4.211 2.55e-05 ***
     CE.Fat.Level            0.5281     0.1639   3.223  0.00127 ** 
     CE.Stom.Layering1      -1.4274     0.7235  -1.973  0.04851 *  
     BS.BHBA.1.21            0.3357     0.3623   0.926  0.35421    
     CE.Lame1                0.5142     0.4140   1.242  0.21421    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 5
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +  
     CE.Fat.Level + CE.Stom.Layering + CE.Lame + (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     476.1    514.3   -229.1    458.1      503 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -2.8744 -0.3766 -0.2396  0.2499  5.3882 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.655    1.287   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                           Estimate Std. Error z value Pr(>|z|)    
     (Intercept)            -1.0811     0.7151  -1.512  0.13058    
     BS.MS.Date.Difference  -0.1870     0.1511  -1.238  0.21584    
     MS.DIM                 -0.2266     0.1474  -1.537  0.12426    
     FPR.1.41                0.9372     0.3096   3.028  0.00247 ** 
     MS.Acetone.Log          0.9320     0.2002   4.655 3.23e-06 ***
     CE.Fat.Level            0.5236     0.1636   3.201  0.00137 ** 
     CE.Stom.Layering1      -1.3590     0.7154  -1.900  0.05747 .  
     CE.Lame1                0.5035     0.4134   1.218  0.22331    
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 6
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ BS.MS.Date.Difference + MS.DIM + FPR.1.4 + MS.Acetone.Log +      
     CE.Fat.Level + CE.Stom.Layering + (1 |CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     475.5    509.4   -229.8    459.5      504 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -2.8898 -0.3695 -0.2283  0.2441  4.8818 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.959    1.4     
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                           Estimate Std. Error z value Pr(>|z|)    
     (Intercept)            -1.1023     0.7373  -1.495  0.13491    
     BS.MS.Date.Difference  -0.1900     0.1558  -1.220  0.22262    
     MS.DIM                 -0.2313     0.1508  -1.534  0.12513    
     FPR.1.41                0.9730     0.3176   3.064  0.00218 ** 
     MS.Acetone.Log          0.9652     0.2061   4.682 2.84e-06 ***
     CE.Fat.Level            0.5249     0.1691   3.103  0.00192 ** 
     CE.Stom.Layering1      -1.3463     0.7355  -1.830  0.06718 .  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 7
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ MS.DIM + FPR.1.4 + MS.Acetone.Log + CE.Fat.Level +      
     CE.Stom.Layering + (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     475.1    504.7   -230.5    461.1      505 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -2.8942 -0.3766 -0.2349  0.2394  4.7343 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.901    1.379   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                       Estimate Std. Error z value Pr(>|z|)    
     (Intercept)        -1.1707     0.7295  -1.605  0.10853    
     MS.DIM             -0.2304     0.1501  -1.535  0.12486    
     FPR.1.41            0.9851     0.3151   3.126  0.00177 ** 
     MS.Acetone.Log      0.9713     0.2045   4.750 2.03e-06 ***
     CE.Fat.Level        0.5494     0.1677   3.276  0.00105 ** 
     CE.Stom.Layering1  -1.2718     0.7257  -1.753  0.07967 .  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 8
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ FPR.1.4 + MS.Acetone.Log + CE.Fat.Level + CE.Stom.Layering +      
     (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     475.5    501.0   -231.8    463.5      506 

     Scaled residuals: 
        Min      1Q  Median      3Q     Max 
     -2.5832 -0.3903 -0.2460  0.2628  5.3980 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 1.73     1.315   
     Number of obs: 512, groups:  CowID:Farm.No, 325

     Fixed effects:
                       Estimate Std. Error z value Pr(>|z|)    
     (Intercept)        -1.1282     0.7179  -1.572 0.116038    
     FPR.1.41            0.9295     0.3061   3.037 0.002389 ** 
     MS.Acetone.Log      1.0031     0.2010   4.991 6.02e-07 ***
     CE.Fat.Level        0.5580     0.1650   3.381 0.000722 ***
     CE.Stom.Layering1  -1.2223     0.7150  -1.709 0.087377 .  
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

#### NEFA Multiple Regression - Step 9 - Final Model
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

#### NEFA Multiple Regression - Step 10
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
#### NEFA Multiple Regression - Step 11
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ MS.Acetone.Log + CE.Fat.Level + MS.Oleic + (1 |      CowID:Farm.No)
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

#### NEFA Multiple Regression - Step 12
     Generalized linear mixed model fit by maximum likelihood (Laplace Approximation) ['glmerMod']
     Family: binomial  ( logit )
     Formula: BS.NEFA.0.7 ~ CE.Fat.Level + MS.Oleic + (1 | CowID:Farm.No)
     Data: sub4nc_FA

      AIC      BIC   logLik deviance df.resid 
     380.7    396.9   -186.4    372.7      412 

     Scaled residuals: 
       Min      1Q  Median      3Q     Max 
     -3.1546 -0.3525 -0.2184  0.2270  2.6637 

     Random effects:
     Groups        Name        Variance Std.Dev.
     CowID:Farm.No (Intercept) 2.01     1.418   
     Number of obs: 416, groups:  CowID:Farm.No, 258

     Fixed effects:
             Estimate Std. Error z value Pr(>|z|)    
     (Intercept)   -1.8371     0.3374  -5.445 5.18e-08 ***
     CE.Fat.Level   0.4136     0.1870   2.212    0.027 *  
     MS.Oleic       1.4932     0.2650   5.635 1.75e-08 ***
     ---
     Signif. codes:  0 ‘***’ 0.001 ‘**’ 0.01 ‘*’ 0.05 ‘.’ 0.1 ‘ ’ 1

## NEFA Odds Ratio's, Confidence Intervals, and Effect Plots
                       OR      2.5 %     97.5 %     
     (Intercept)  1.5122676 0.05850544  0.2715485
     CE.Fat.Level 4.4512724 1.06472866  2.2943550
     MS.Oleic     0.1592734 2.86633221  9.0312020


