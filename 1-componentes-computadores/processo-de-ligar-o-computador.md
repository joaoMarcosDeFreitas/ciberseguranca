# Processo de Ligar o Computador

---

## 1. Botão de Inicio:

- Ao ligar um computador, um sinal é mandado ao **PSU (Power Supply Unit)** permitindo que então ele forneça energia. É como se ao dormir nosso corpo parasse de bombear sangue e ao acordar ele mandasse um sinal ao coração dizendo 'podemos bombear agora'.

## 2. Inicio do Firmware (BIOS / UEFI):

- Ao começar a bombear sangue, o corpo então começa a 'rodar' seus principais órgãos, porém ainda não temos consciência, e no PC com essa analogia seriam nosso componentes rodando, porém ainda não estão inicializados. Quem é responsável pelo controle de inicialização dos componentes é a **UEFI (Unified Extensible Firmware Interface)** ou **BIOS (Basic Input/Output System)**. Ambos são parecidos e tem funções semelhantes, porém a UEFI é mais moderna e substituiu o BIOS por oferecer mais proteção, interface e velocidade.

## 3. Testes e Verificações Após Ligar:

- Após a inicialização, o ****UEFI (ou BIOS)**** começa então uma verificação dos componentes, para observar se estão presentes, ativos e funcionando. Caso por algum motivo ele encontre uma irregularidade, algum sinal é enviado, seja um alarme na tela,  beeps, LEDs, entre outros. UEFI executa **Power-On Self Test (POST)**.

## 4. Escolher Boot Device:

- Após o sistema estar ligado e rodando, o **UEFI (ou BIOS)** possuem uma lista ordenada que procura exatamente aonde a nossa rotina de inicialização (bootup routine) está localizada para que possa ser executada.

## 5. Inicializar o Bootloader: 

- Após localizar o boot device o bootloader inicia, o bootloader envia o nosso **SO (Sistema Operacional)** do boot selecionado para a **RAM (Random Access Memory)**. Após ser transferido para lá, o **UEFI (ou BIOS)** passa o controle dos componentes para o SO.

---