# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Two-Stage Hard Thresholding (TSHT) Use TSHT (RobustIV) With (In) R Software
install.packages("RobustIV")
library("RobustIV")
TSHT = read.csv("https://raw.githubusercontent.com/timbulwidodostp/TSHT/main/TSHT/TSHT.csv",sep = ";")
# Estimation Two-Stage Hard Thresholding (TSHT) Use TSHT (RobustIV) With (In) R Software
Y <- TSHT[,"Y"]
D <- TSHT[,"D"]
Z <- as.matrix(TSHT[,c("Z.1","Z.2","Z.3","Z.4","Z.5","Z.6","Z.7","Z.8")])
X <- as.matrix(TSHT[,c("age","sex")])
TSHT <- TSHT(Y=Y,D=D,Z=Z,X=X)
summary(TSHT)
# Two-Stage Hard Thresholding (TSHT) Use TSHT (RobustIV) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished