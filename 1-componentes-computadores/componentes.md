# Componentes Computadores

---

## 1. Motherboard (Placa-Mãe):

- **O que é:** É uma placa de circuito eletrônico grande, que serve para fazer os componentes do computador se 'conectarem'. Conecta diversos componentes do computador. Funciona como um ponto central de comunicação do computador.

- **Como é formada:**
    1. **PCB (Printed Circuit Board)** -> É a própria placa, feita de material isolante, é nela que conectamos os componentes eletrônicos.
    2. **Trilhas de Cobre** -> São as trilhas de cobre que levam eletricidade e energia para os componentes.
    3. **Barramentos** -> Servem para que os componentes possam trocar dados entre si:
        -  Dentre eles temos:
            - **PCIe (PCI express / Peripheral Component Interconnect Express)** -> Padrão de comunicação de alta velocidade para conectar dispositivos à placa-mãe. Lane: Canal individual de comunicação PCIe. Por isso que existem as PCIe x1, x4, x8, x16.
                - Usado para:
                    - GPU (Placas de Vídeo)
                    - Placas de rede
                    - SSDs NVMe
                    - Placas de extensão
            - **SATA (Serial Advanced Technology Attachment)** -> Padrão de comunicação usado principalmente para HDDs e SSDs SATA.
                - Fisicamente temos:
                    - Porta SATA na placa-mãe
                    - Cabo SATA de dados
                    - Controlador SATA
            - **USB (Universal Serial Bus)** -> Padrão de comunicação usado para conectar periféricos e dispositivos externos. Transporta dados e energia. Podem ser usados para transportar códigos malicioso, malwares entre outros dados perigosos.
            - **Interfaces de Memória**
    4. **Soquete da CPU** -> É onde conecta eletrônicamente a placa-mãe com o processador.
    5. **Slots de RAM** -> Local/Locais para conectar a(s) memória(s) RAM (Random Access Memory). 
    6. **Chipset** -> Conjunto de controladores da placa-mãe, gerencia determinadas comunicações entre CPU, armazenamento, USB, PCIe e outros dispositivos. Auxilia no controle de comunicações. Nos computadores modernos, algumas funções antes atribuídas aos chipsets estão agora na CPU.
    7. **M.2** -> Formato físico utilizado para instalar dispositivos diretamente na placa-mãe, principalmente SSDs.
        - Dentre os usos temos:
            - **SSD M.2 SATA:** Utiliza o formato físico M.2 e a interface de comunicação SATA.
            - **SSD M.2 NVMe:** Utiliza o formato físico M.2, comunicação através do PCIe e o protocolo NVMe.
    8. **NVMe (Non-Volatile Memory Express)** -> Padrão de comunicação desenvolvido especificamente para memórias não voláteis (SSDs). É mais rápido que o SATA. Substitui o SATA pela sua velocidade e baixa latência.
    9. **VRM (Voltage Regulator Module)** -> Circuito que regula a tensão elétrica fornecida a CPU e outros componentes. `Não faz parte diretamente da segurança, porém faz parte da estrutura elétrica da placa`.
    10. **Conectores de Energia** -> Recebem a energia fornecida pelo PSU (Power Supply Unit) e alimentam a placa-mãe e seus componentes.
    11. **BIOS (Basic Input/Output System)** -> Firmware tradicional usado para inicializar o hardware e iniciar o processo de boot. Usado para testar componentes inicialmente, localizar o sistema operacional entre outras tarefas. Firmwares comprometidos podem atingir o computador em uma linguagem muito abaixo do nível do sistema operacional.
    12. **UEFI (Unified Extensible Firmware Interface)** -> Firmware moderno que substituiu amplamente o BIOS em PCs modernos. Oferece mecanismos de segurança (Secure Boot), é mais rápido que o BIOS, e possui interface gráfica. Firmwares comprometidos podem atingir o computador em uma linguagem muito abaixo do nível do sistema operacional.
        - **Secure Boot** -> Verifica se os componentes a serem inicializados possuem assinaturas confiáveis, antes de inicializá-los. Impede que softwares não autorizados inicializem durante o boot.
    13. **TPM (Trusted Platform Module)** -> Módulo de segurança que criptografa chaves e informações relacionadas a integridade do sistema.
    14. **DMA (Direct Memory Access)** -> Tecnologia que permite que alguns dispositivos acessem a RAM diretamente, sem precisar da CPU diretamente na atuação. 
    15. **IOMMU (Input-Output Memory Management Unit)** -> Controlam quem acessa a memória, usado para evitar quem usa e acessa a memória via DMA.

## 2. CPU (Central Processing Unit) / Processador:

- **O que é:** Assim como nosso cérebro, o processador executa instruções e tarefas. Possui muitos núcleos para trabalhar com tarefas em paralelo e fica localizada em um soquete da CPU (item 4 no tópio ## 1. Motherboard) na placa-mãe.

## 3. RAM (Random Access Memory):

- **O que é:** Assim como nossa memória enquanto trabalhamos, muitas vezes precisamos guardar informações rápidas para uso naquele momento em que estamos atarefados. Dessa forma, a RAM funciona exatamente como essas memórias de curto prazo, pois ela guarda informações relevantes durante o momento em que o PC fica ligado, a CPU precisa e acessa essas informações. Após desligarmos o PC, seu conteúdo vai embora.

## 4. Storage SSD (Solid State Drive) e HDD (Hard Disk Drive):

- **O que é:** Em contra partida do que vimos em `3. RAM (Random Access Memory)` esses armazenamentos chamados SSD e HDD são nossas memórias de longo prazo, é como se fosse as informações que você guarda por anos. HDDs usam tecnologia mais antiga, possuindo escrituras físicas, de fato se movendo para registrar as informações, limitando assim sua performance (que fica mais lenta). Por outro lado, SDDs são mais modernos e não precisam se mover para registrar informações, usam chips de memória (o que fica muito mais rápido). HDDs ainda tem seu lugar no mercado, por seu baixo custo para alto nível de armazenamento. Ambos usam SATA ou PCIe para se conectar (ambos barramentos estudados em `1. Motherboard (Placa-Mãe)`). Exemplos muito comuns hoje em dia são: SSD M.2 NVMe e SSD M.2 SATA (ainda que NVMe seja mais veloz que o SATA).

## 5. Network Adapter (Placa de rede):

- **O que é:** Funciona como nossas cordas vocais, que se comunicam com outras pessoas, o network adapter (placa de rede) faz seu computador se conectar a rede, podendo ser via cabo (ethernet) ou sem cabo (wireless). Muitas vezes já vem embutida na motherboard (placa-mãe), porém também existe a forma de conectar através de PCIe com cartão de extensão. A entrada para ethernet pode ser vista em computadores analisando de fora.

## 6. PSU (Power Supply Unit):

- **O que é:** Assim como nosso coração bombeia sangue para todo o corpo, o PSU (Power Supply Unit) distribui a energia para todos os componentes. É essencial para funcionamento do sistema e quando um componente precisa de mais energia do que o PSU pode fornecer, o sistema vai falhar ou apresentar problemas. Existem varios conectores para distribuição de energia.

## 7. GPU (Graphics Processing Unit):

- **O que é:** É como nosso córtex visual, os olhos pegam as informações e o córtex transforma em imagens, o sistema e seus programas enviam informações a GPU (Graphics Processing Unit) e ela então faz um output visual do que recebe a um monitor. GPUs são conectadas via PCIe diretamente na motherboard (placa-mãe).

## 8. I/O (Input/Output):

- **O que é:** São os componentes que se conectam ao PC, inputs podem ser mouses, teclados, fones, entre outros. Já os outputs podem ser monitores, impressoras, caixas de som, entre outros. Todos esses podem ser conectados com algumas formas, as vias mais famosas são USB, HDMI e DisplayPort.

---