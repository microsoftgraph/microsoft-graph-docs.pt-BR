---
title: Conjuntos de dados, regiões e coletores compatíveis com o Microsoft Graph Data Connect
description: Descreve os conjuntos de dados suportados e tipos de armazenamento de destino que podem ser usados com o Microsoft Graph Data Connect.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: fd4fbac34f4b03a3802de4834f0c02045d57c4ea
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547622"
---
# <a name="datasets-regions-and-sinks-that-microsoft-graph-data-connect-supports"></a>Conjuntos de dados, regiões e coletores compatíveis com o Microsoft Graph Data Connect

Microsoft Graph Data Connect dá suporte a vários conjuntos de dados, regiões de dados e locais de armazenamentos do Microsoft Azure. Este tópico descreve os conjuntos de dados suportados e como acessar os esquemas de conjunto de dados, regiões suportadas do Microsoft 365 e do Microsoft Azure, e os locais de armazenamento que a Conexão de Dados usa por meio do Azure Data Factory.

Se desejar solicitar suporte para conjuntos de dados, regiões ou coletores adicionais, informe-nos no fórum de ideias da[Plataforma de Desenvolvedor do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

## <a name="datasets"></a>Conjuntos de dados

A conexão de dados suporta hoje os seguintes conjuntos de dados. Para exibir esquemas de cada conjunto de dados, crie um novo conjunto de dados no Azure Data Factory e use a guia Esquema para exibi-los. 

|Nome do conjunto de dados|Descrição|
|-------------|-----------|
|BasicDataSet_v0.Contact_v0|Contém informações de contato do catálogo de endereços de cada usuário. O esquema para esses entidades é semelhante ao [esquema de contatos pessoais do Microsoft Graph](/graph/api/resources/contact).| 
|BasicDataSet_v0.Event_v0|Contém os eventos do calendário de cada usuário. O esquema para essas entidades é semelhante ao [esquema do calendário de eventos do Microsoft Graph](/graph/api/resources/event).| 
|BasicDataSet_v0.Message_v0|Contém a mensagem na caixa de correio de cada usuário. O esquema para essas entidades é semelhante ao [esquema de mensagens do Microsoft Graph](/graph/api/resources/message).| 
|BasicDataSet_v0.SentItem_v0|Contém as mensagens enviadas da caixa de correio de cada usuário. O esquema para essas entidades é semelhante ao [esquema de mensagens do Microsoft Graph](/graph/api/resources/message).| 
|BasicDataSet_v0.User_v0|Contém informações de usuário (NomeDeExibição, Nome UPN e assim por diante).| 
|BasicDataSet_v0.MailboxSettings_v0|Contém as configurações da caixa de correio de cada usuário. O esquema para essas entidades corresponde ao [esquema de configuração da caixa de correio do Microsoft Graph](/graph/api/resources/mailboxsettings).| 
|BasicDataSet_v0.MailFolder_v0|Contém as pastas de email da caixa de correio de cada usuário. O esquema para essas entidades corresponde ao [esquema das pastas de email do Microsoft Graph](/graph/api/resources/mailfolder).|
|BasicDataSet_v0.Manager_v0|Contém as informações de usuário para o gerenciador de cada usuário. O esquema para essas entidades corresponde ao [esquema do usuário do Microsoft Graph](/graph/api/resources/user).|
|BasicDataSet_v0.DirectReport_v0|Contém informações de usuário sobre funcionários que se reportam diretamente a cada usuário. O esquema para essas entidades corresponde ao [esquema do usuário do Microsoft Graph](/graph/api/resources/user).|
|BasicDataSet_v0.CalendarView_v0|O esquema para essas entidades corresponde ao [esquema do usuário do Microsoft Graph](https://developer.microsoft.com/graph/docs/api-reference/v1.0/resources/events).|
|BasicDataSet_v0.User_v1|Esta tabela contém informações do usuário. O esquema para essas entidades corresponde ao [esquema do usuário do Microsoft Graph](/graph/api/resources/user).|
|BasicDataSet_v0.Contact_v1|Contém informações de contato do catálogo de endereços de cada usuário. O esquema para esses entidades corresponde ao [esquema de contatos pessoais do Microsoft Graph](/graph/api/resources/contact).|
|BasicDataSet_v0.Event_v1|Contém os eventos do calendário de cada usuário. O esquema para essas entidades corresponde ao [esquema do calendário de eventos do Microsoft Graph](/graph/api/resources/event).|
|BasicDataSet_v0.Message_v1|Contém a mensagem na caixa de correio de cada usuário. O esquema para essas entidades corresponde ao [esquema de mensagens do Microsoft Graph](/graph/api/resources/message).|
|BasicDataSet_v0.SentItem_v1|Contém a mensagem enviada da caixa de correio de cada usuário. O esquema para essas entidades corresponde ao [esquema de mensagens do Microsoft Graph](/graph/api/resources/message).|

## <a name="regions"></a>Regiões

A Conexão de Dados dá suporte à extração de dados de diversas regiões do Microsoft 365. Para migrar os dados com sucesso do centro de dados do Microsoft 365 para seu armazenamento do Microsoft Azure, a instância do Azure Data Factory e o local de armazenamento do Azure devem mapear para uma região com suporte para o local dos dados do Microsoft 365. A tabela a seguir indica quais regiões do Microsoft 365 têm suporte e as regiões do Azure correspondentes necessárias para a movimentação de dados. 

| Região do Office                    | Região do Azure                                |
|----------------------------------|---------------------------------------------|
| **América do Norte**                | Leste dos EUA<br/>Leste 2 dos EUA<br/>Centro dos EUA<br/>Centro-Norte dos EUA<br/>Centro-Sul dos EUA<br/>Centro-Oeste dos EUA<br/>Oeste dos EUA<br/>Oeste 2 dos EUA|
| **Europa**                       | Norte da Europa<br/>Europa Ocidental|
| **Ásia – Pacífico**                 | Leste da Ásia<br/>Sudeste da Ásia|
| **Austrália**                    | Leste da Austrália<br/>Sudeste da Austrália|

## <a name="sinks"></a>Coletores

Coletores são os locais de saída que o Data Factory usa para colocar os dados no armazenamento do Azure. O Data Connect é compatível agora com os seguintes tipos de coletores:

- Azure Data Lake Storage Gen2 (ADLS Gen2)
- Armazenamento de Blob do Azure
- Azure Data Lake Storage Gen1 (ADLS Gen1)

Os coletores possuem as seguintes características: 

- Os arquivos de saída serão no formato Linhas JSON. O formato de saída foi corrigido e não há suporte para modificar o formato de saída. No entanto, você pode usar o Azure Data Factory para copiar o resultado de um pipeline do Data Connect para outro mecanismo de armazenamento (como o Banco de Dados SQL do Azure).
- A autenticação da Entidade de Serviço é o único mecanismo de autenticação com suporte para todos os tipos de coletores em uma atividade de cópia com o Microsoft 365 como a origem.
- Ao usar o Armazenamento de Blob do Azure como coletor, certifique-se de que o aplicativo tem acesso de Colaborador de Dados de Armazenamento de Blob para o local de Armazenamento de Blob do Azure.

## <a name="next-steps"></a>Próximos passos

Para saber mais sobre como criar pipelines do Data Connect como parte do Azure Data Factory, confira a [documentação do conector do Office 365 do Azure Data Factory](/azure/data-factory/connector-office-365).