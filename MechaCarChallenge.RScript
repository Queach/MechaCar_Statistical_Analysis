library(dplyr)
mecha_car <- read.csv('MechaCar_mpg.csv',stringsAsFactors = F)
lm(mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD,data=mecha_car)
summary(lm(mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD,data=mecha_car))

susp_coil <- read.csv('Suspension_Coil.csv',stringsAsFactors = F)
total_summary <- susp_coil %>% summarize(Mean=mean(PSI),Median=median(PSI), Variance=var(PSI), SD=sd(PSI), .groups = 'keep')
lot_summary <- susp_coil %>% group_by(Manufacturing_Lot) %>% summarize(Mean=mean(PSI),Median=median(PSI), Variance=var(PSI), SD=sd(PSI), .groups = 'keep')
?t.test()

t.test(susp_coil$PSI,mu=1500) #compare sample versus population mean

lot1 <- susp_coil %>% filter(Manufacturing_Lot == "Lot1") %>% summarise(PSI=PSI)
lot2 <- susp_coil %>% filter(Manufacturing_Lot == "Lot2") %>% summarise(PSI=PSI)
lot3 <- susp_coil %>% filter(Manufacturing_Lot == "Lot3") %>% summarise(PSI=PSI)
t.test(lot1$PSI, mu=1500) 
t.test(lot2$PSI, mu=1500)
t.test(lot3$PSI, mu=1500)

