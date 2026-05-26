# dio-aws-ec2



### O que são instancias EC2 ?

EC2 -- Elastic Compute Cloud, são as maquinas virtuais na AWS, podendo ser com sistema operacional Windows ou Linux.

Uma EC2 é composta por:

* CPU
* Memória
* Disco 
* Rede
* Sistema operacional


No modelo Cloud, uma EC2 é do tipo IAAS ou seja, quando criamos um EC2 estamos utilizando o tipo infraestrutura como serviço.

E qual seria nossa responsabilidade sobre este recurso ?

Seria nso aplicativos, dados e conexões.


Como escolher a EC2 correta para minha aplicação ?

Escolher a instancia correta na AWS é crucial para garantir eficiencia, escalabilidade e economia nos gastos com nuvem.

![[Pasted image 20260525172550.png]]


### Os tipos de instancias EC

Cada tipo de instancia oferece diferentes recursos de computação como memória e armazenamento e é agrupado em familais de instancias com base nesses recursor.

![[Pasted image 20260525173349.png]]
![[Pasted image 20260525174241.png]]
![[Pasted image 20260525174312.png]]

### Otimização de recursos 

Quando falamos de otimizaçao de recursos, estamos apontando para "custo", ou seja, otimizar recurso é poupar custos na AWS.
Mesmo otimizando um recurso computacional, onde melhoramos o desempenho do sistema, estamos poupando custo, pois isto traz ganho para a nossa solução na nuvem.


![[Pasted image 20260525211054.png]]


### Criaçao de imagens

O que é a imagem de maquina da Amazon (AMI) ?

No Amazon EC2 ( Elastic Compute Cloud ), uma AMI (Amazon Machine Image) é uma imagem de máquina virtual pré-configurada, que inclui as informações necessárias para iniciar uma instancia, como sistema operativo, o servidor de aplicaçoes e as aplicaçoes.

### Criação e uso de imagens AMI

1. Criação: As AMIs podem ser criadas a partir de instancias em execução ou paradas. Isto permite-lhe capturar um instantaneo do seu ambiente configurado.

2. AMIs publicas e privadas: A AWS fornece uma variedade de AMIs publicas que podem ser usadas, ou voce pode criar e usar suas proprias AMIs privadas para segurança e personalização.

3. Personalização: é possivel personalizar uma instancia ( instalar software, configurar definições) e , em seguida, criar uma AMI a partir dela. Isso facilita a replicação do seu ambiente.

4. Iniciar instancias: Para executar instancias no EC2, seleciona uma AMI. A AMI fornece as informações necessárias para iniciar a instancia, como volume do dispositivo raiz e as permissoes de inicialização.

5. Tipos de AMI: Existem diferentes tipos de AMIs, incluindo Amazon Linux, Windows e outros, Escolhe-se uma AMI com base nos requisitos da aplicação e do sistema.

Entender as AMIs é crucial para gerenciar e implantar instancias no EC2 de forma eficiente. Elas fornecem uma base para criação de ambientes consistentes e reproduziveis na nuvem.



Amazon EBS - Elastic Block Store, nada mais é do que uma storage altamente confiavel que pode ser anexado em qualquer instancia EC2. Toda instancia possui um volume de armazenamento.
Agora com EBS conseguimos ter a capacidade de expansão de forma rápida, com apenas alguns clicks.


### Snapshot em EBS 

Para entendermos de fato o que sao os snapshots EBS, para isto devemos primeiro compreender os componentes os serviços de nuvem da Amazon:
O Amazon Elastic Compute Cloud (EC2) é um serviço da Amazon que fornece capacidade de computaçao escalavel na nuvem do amazon web services atraves de maquinas virtuais, conhecidas como instancias.

O Amazon Elastic Block Store é um serviço para fornecer armazenamento em bloco fiável ( também conhecido como volumes ou discos rígiso). Foi concebido para ser utilizado com instancias do Amazon Elastic Compute Cloud


Regios: São areas geograficas contendo varias availability zones

Availability Zones : São data centers independentes fisicamente, mas conectados logicamente, para garantir alta disponibilidade.


Amazon S3 ( Amazon Simple Storage Service ) é um serviço de armazenamento de objetos em nuvem oferecidos pela AWS.

É ideal para armazenar, organizar e recuperar grandes volumes de dados de forma segura e escalavel.

O amazon S3 possui algumas classes de storages onde conseguimos economizar nos custos.

Um exemplo muito bom para entendermos as diferentes classes do S3 é o exemplo do exame de Hospital.

![[Pasted image 20260525213227.png]]

![[Pasted image 20260525213521.png]]

Podemos utilizar regra de ciclo de vida para definir a forma como o Amazon S3 gere os objetos durante o seu tempo de vida.

O lifecycle permite fazer a transição de objetos e migrar automaticamente para classe Glacier.


