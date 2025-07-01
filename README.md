# Desafio DIO AZ-104: Gerenciamento de Máquinas Virtuais no Azure

## Introdução

Este repositório é um material de apoio para o desafio do curso AZ-104 da DIO, focado no gerenciamento de máquinas virtuais (VMs) no Microsoft Azure. O objetivo é consolidar resumos, anotações e dicas práticas sobre o uso do Azure, servindo como um guia rápido para estudos e futuras implementações.

## Objetivos de Aprendizagem

Ao explorar este repositório, você será capaz de:

*   **Aplicar conceitos:** Entender e aplicar os conceitos de gerenciamento de VMs em um ambiente prático do Azure.
*   **Documentar processos:** Aprender a documentar processos técnicos de forma clara e estruturada, essencial para a colaboração e o compartilhamento de conhecimento.
*   **Utilizar o GitHub:** Dominar o uso do GitHub como uma ferramenta eficaz para versionamento e compartilhamento de documentação técnica.

## Estrutura do Repositório

Este repositório está organizado da seguinte forma:

*   `README.md`: Este arquivo, contendo a introdução, objetivos, estrutura do repositório, e o conteúdo principal sobre o gerenciamento de VMs no Azure.
*   `/images`: Uma pasta opcional para armazenar capturas de tela relevantes que ilustram os passos e conceitos abordados.
*   `anotacoes.md` (Exemplo): Um arquivo Markdown adicional para anotações mais detalhadas ou específicas sobre tópicos relacionados.

## Gerenciamento de Máquinas Virtuais no Microsoft Azure

O Microsoft Azure oferece uma plataforma robusta para a criação e gerenciamento de máquinas virtuais, permitindo que você execute uma variedade de cargas de trabalho na nuvem. As VMs no Azure são uma das principais ofertas de Infraestrutura como Serviço (IaaS), proporcionando flexibilidade e escalabilidade.

### Criação de Máquinas Virtuais

A criação de uma VM no Azure envolve a seleção de vários parâmetros para atender às suas necessidades específicas. Os passos básicos incluem:

1.  **Escolha da Imagem:** Selecionar o sistema operacional (Windows Server, Ubuntu, CentOS, etc.) e a versão da imagem base.
2.  **Tamanho da VM:** Definir o tamanho da VM, que determina o número de vCPUs, a quantidade de memória, e o tipo de disco (HDD ou SSD). O Azure oferece uma vasta gama de tamanhos, otimizados para diferentes cargas de trabalho (uso geral, otimizadas para computação, otimizadas para memória, etc.).
3.  **Configuração de Rede:** Configurar a rede virtual (VNet), sub-rede, endereço IP público (se necessário), e grupos de segurança de rede (NSGs) para controlar o tráfego de entrada e saída.
4.  **Discos:** Escolher o tipo de disco (Standard HDD, Standard SSD, Premium SSD) e o tamanho do disco do sistema operacional, além de adicionar discos de dados, se necessário.
5.  **Autenticação:** Definir o método de autenticação, que pode ser nome de usuário e senha ou chave SSH para VMs Linux.

### Gerenciamento do Ciclo de Vida da VM

Após a criação, o gerenciamento de uma VM no Azure envolve diversas operações:

*   **Iniciar/Parar/Reiniciar:** Controlar o estado de execução da VM. Parar uma VM desaloca os recursos de computação, o que pode economizar custos, mas o disco e o IP público (se for estático) ainda são cobrados.
*   **Redimensionar:** Alterar o tamanho da VM para ajustar o desempenho ou os custos. Isso pode ser feito para cima (scale up) ou para baixo (scale down).
*   **Capturar Imagem:** Criar uma imagem personalizada de uma VM para implantar novas VMs com a mesma configuração.
*   **Backup e Recuperação:** Configurar políticas de backup para proteger os dados da VM e garantir a recuperação em caso de falha.
*   **Monitoramento:** Utilizar o Azure Monitor para coletar e analisar métricas de desempenho, logs e alertas, garantindo a saúde e a disponibilidade da VM.
*   **Segurança:** Implementar medidas de segurança como Azure Security Center, Azure Firewall, e Just-in-Time VM Access para proteger suas VMs contra ameaças.

### Dicas e Boas Práticas

*   **Otimização de Custos:** Utilize VMs de tamanho adequado para sua carga de trabalho. Considere o uso de VMs Spot para cargas de trabalho tolerantes a interrupções e reserve instâncias para economias significativas em longo prazo.
*   **Automação:** Use Azure Resource Manager (ARM) templates, Azure CLI, ou Azure PowerShell para automatizar a implantação e o gerenciamento de VMs, garantindo consistência e reduzindo erros manuais.
*   **Rede:** Configure NSGs de forma granular para permitir apenas o tráfego necessário, aumentando a segurança. Utilize Azure Bastion para acesso seguro a VMs sem expor IPs públicos.
*   **Discos:** Prefira Premium SSDs para cargas de trabalho de produção que exigem alta performance. Considere o uso de discos efêmeros para caches ou dados temporários.
*   **Monitoramento e Alertas:** Configure alertas para métricas críticas (uso de CPU, memória, espaço em disco) para ser proativo na resolução de problemas.

## Recursos Úteis

*   **Documentação Oficial:**
    *   [Gerenciar máquinas virtuais do Azure - Artigo no Microsoft Learning](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/overview )

*   **Materiais Complementares sobre GitHub:**
    *   [GitHub Quick Start - Repositório com Link para Aulas de Git e GitHub](https://github.com/githubtraining/quickstart )
    *   [GitBook: Formação GitHub Certification - Material textual sobre GitHub](https://gitbook.com/ )
    *   [Documentação do GitHub - Guia completo para uso do GitHub](https://docs.github.com/ )
    *   [GitHub Markdown - Guia específico para Markdown no GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax )

---


**Data:** 7 de janeiro de 2025
