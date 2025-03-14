# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Generalized Synthetic Control Method Use gsynth With (In) R Software
install.packages("gsynth")
library("gsynth")
gsynth = read.csv("https://raw.githubusercontent.com/timbulwidodostp/gsynth_r/main/gsynth/gsynth.csv",sep = ";")
# Estimation Generalized Synthetic Control Method Use gsynth With (In) R Software
gsynth <- gsynth(Y ~ D + X1 + X2, data = gsynth, parallel = FALSE, index = c("id","time"), force = "two-way", CV = TRUE, r = c(0, 5), se = FALSE) 
print(gsynth)
# Generalized Synthetic Control Method Use gsynth With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished