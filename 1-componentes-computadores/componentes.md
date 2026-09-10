# Componentes Computadores

---

## 1. Motherboard (Placa-Mãe):

- **O que é:** É uma placa de circuito eletrônico grande, que serve para fazer os componentes do computador se 'conectarem'.

- **O que faz:** Conecta diversos componentes do computador. Funciona como um ponto central de comunicação do computador.

- **Como é formada:**
    1. **PCB (Printed Circuit Board)** -> É a própria placa, feita de material isolante, é nela que conectamos os componentes eletrônicos.
    2. **Trilhas de Cobre** -> São as trilhas de cobre que levam eletricidade e energia para os componentes.
    3. **Barramentos** -> Servem para que os componentes possam trocar dados entre si:
        -  Dentre eles temos:
            - **PCIe (PCI express / Peripheral Component Interconnect Express)** -> Padrão de comunicação de alta velocidade para conectar dispositivos à placa-mãe.
                - Usado para:
                    - GPU (Placas de Vídeo)
                    - Placas de rede
                    - SSDs NVMe
                    - Placas de extensão
                - **Lane:** Canal individual de comunicaão PCIe. Por isso que existem as PCIe x1, x4, x8, x16.
            - **SATA (Serial Advanced Technology Attachment)** -> Padrão de comunicação usado principalmente para HDDs e SSDs SATA.
                - Fisicamente temos:
                    - Porta SATA na placa-mãe
                    - Cabo SATA de dados
                    - Controlador SATA
                - OBS: SATA é a tecnologia. Não é o cabo ou a porta em si.
            - **USB (Universal Serial Bus)** -> Padrão de comunicação usado para conectar periféricos e dispositivos externos. Transporta dados e energia. Podem ser usados para transportar códigos malicioso, malwares entre outros dados perigosos.
            - **NVMe (Non-Volatile Memory Express)** -> Padrão de comunicação desenvolvido especificamente para memórias não voláteis (SSDs). É mais rápido que o SATA. Substitui o SATA pela sua velocidade e baixa latência.
            - **Interfaces de Memória**
    4. **Soquete da CPU** -> É onde conecta eletrônicamente a placa-mãe com o processador.
    5. **Slots de RAM** -> Local/Locais para conectar a(s) memória(s) RAM (Random Access Memory). 
    6. **Chipset** -> Conjunto de controladores da placa-mãe, gerencia determinadas comunicações entre CPU, armazenamento, USB, PCIe e outros dispositivos. Auxilia no controle de comunicações. Nos computadores modernos, algumas funções antes atribuídas aos chipsets estão agora na CPU.
    7. **M.2** -> Formato físico utilizado para instalar dispositivos diretamente na placa-mãe, principalmente SSDs.
    9. **VRM (Voltage Regulator Module)** -> Circuito que regula a tensão elétrica fornecida a CPU e outros componentes. `Não faz parte diretamente da segurança, porém faz parte da estrutura elétrica da placa`.
    10. **Conectores de Energia** -> Recebem a energia fornecida pelo PSU (Power Supply Unit) e alimentam a placa-mãe e seus componentes.
    11. **BIOS (Basic Input/Output System)** -> Firmware tradicional usado para inicializar o hardware e iniciar o processo de boot. Usado para testar componentes inicialmente, localizar o sistema operacional entre outras tarefas. Firmwares comprometidos podem atingir o computador em uma linguagem muito abaixo do nível do sistema operacional.
    12. **UEFI (Unified Extensible Firmware Interface)** -> Firmware moderno que substituiu amplamente o BIOS em PCs modernos. Oferece mecanismos de segurança (Secure Boot), é mais rápido que o BIOS, e possui interface gráfica. Firmwares comprometidos podem atingir o computador em uma linguagem muito abaixo do nível do sistema operacional.
        - **Secure Boot** -> Verifica se os componentes a serem inicializados possuem assinaturas confiáveis, antes de inicializá-los. Impede que softwares não autorizados inicializem durante o boot.
    13. **TPM (Trusted Platform Module)** -> Módulo de segurança que criptografa chaves e informações relacionadas a integridade do sistema.
    14. **DMA (Direct Memory Access)** -> Tecnologia que permite que alguns dispositivos acessem a RAM diretamente, sem precisar da CPU diretamente na atuação. 
    15. **IOMMU (Input-Output Memory Management Unit)** -> Controlam quem acessa a memória, usado para evitar quem usa e acessa a memória via DMA.