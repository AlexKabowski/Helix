# HybridOS
Um sistema operacional híbrido experimental, seguro e modular, construído sobre o microkernel seL4 e uma camada baseado no BSD

# Visão Geral
O HybridOS é um projeto de sistema operacional que visa explorar a arquitetura de kernels híbridos, combinando a segurança e o isolamento de um microkernel com a familiaridade e a robustez de um userland Unix-like.

Nosso objetivo é criar uma base de sistema operacional que seja:

Segura: Utilizando o microkernel seL4, que é formalmente verificado para ser seguro.

Modular: Construída a partir de componentes isolados (drivers, servidores, etc.) usando a ferramenta CAmkES.

Compatível: Oferecendo uma camada de serviços BSD-like, facilitando a portabilidade de ferramentas e aplicativos.

# Arquitetura do Sistema
O sistema é construído em camadas, com uma estratégia de licenciamento que reflete a sua modularidade:

Fundaçāo (Kernel): O microkernel seL4 (GPLv2). Esta camada é responsável por gerenciar a comunicação e a segurança entre os componentes.

Camada de Serviços: A camada de serviços, que inclui drivers, servidores de arquivos e bibliotecas essenciais.

# Estado do Projeto
Este projeto está em sua fase inicial de desenvolvimento. Atualmente, o foco está na configuração do ambiente de build, na compreensão do fluxo de inicialização e na criação dos primeiros componentes minimalistas com o CAmkES.

# Como Contribuir
Contribuições são bem-vindas! Se você estiver interessado em colaborar, por favor, leia as instruções de build e a documentação do código. Você pode reportar bugs, sugerir melhorias ou enviar pull requests.
