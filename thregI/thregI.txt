# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fit threshold regression for interval-censored data Use thregI With (In) R Software
install.packages("thregI")
library("thregI")
thregI = read.csv("https://raw.githubusercontent.com/timbulwidodostp/thregI/main/thregI/thregI.csv",sep = ";")
# Estimation Fit threshold regression for interval-censored data Use thregI With (In) R Software
thregI$f.treatment=factor(thregI$treatment)
fit<-thregI(Surv(left, right, type='interval2')~f.treatment|f.treatment, data=thregI)
fit
# Fit threshold regression for interval-censored data Use thregI With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished