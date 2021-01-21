# ubuntu-notes

## Arreglar wifi metodo no 100% revisado
 inxi -Fxz
• driver: "copiar el driver de tu computador"
Es donde dice card-2 driver ese es el driver
• driver: ath9k_htc
• grep [[:alnum:]] /sys/module/ath9k_htc/parameters/*
• echo "options ath9k_htc fwlps=N" | sudo tee /etc/modprobe.d/ath9k_htc.conf
• Reiniciar el computador
