---
title: Conjuntos de dados, regiões e coletores com suporte da Conexão de dados do Microsoft Graph
description: Saiba mais sobre os conjuntos de dados com suporte, regiões do Microsoft 365 e tipos de armazenamento de coletor que você pode usar com a Conexão de Dados do Microsoft Graph.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: b9138bfe4bbbb664deeea463745a264116035fb1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094023"
---
# <a name="datasets-regions-and-sinks-supported-by-microsoft-graph-data-connect"></a>Conjuntos de dados, regiões e coletores com suporte da Conexão de dados do Microsoft Graph

A Conexão de Dados do Microsoft Graph dá suporte a vários conjuntos de dados, regiões de dados e locais de armazenamentos do Microsoft Azure. Este artigo descreve os conjuntos de dados suportados e como acessar os esquemas de conjunto de dados, as regiões do Microsoft Azure e do Microsoft 365 suportadas e os locais de armazenamento que o Data Connect utiliza por meio do Azure Data Factory.

## <a name="datasets"></a>Conjuntos de dados

No momento o Microsoft Graph Data Connect suporta os conjuntos de dados a seguir. Para exibir os esquemas de cada conjunto de dados, crie um novo conjunto de dados no Azure Data Factory e utilize a guia Esquema para exibi-lo.

| Nome do conjunto de dados | Descrição | Amostra | Esquema |
|--------------|-------------|--------|--------|
| BasicDataSet_v0.CalendarView_v0    | Contém os eventos da exibição Calendário.                                        | [CalendarView_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.CalendarView_v0.json)      | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/CalendarView_v0.md) |
| BasicDataSet_v0.Contact_v0         | Contém as informações disponíveis do catálogo de endereços de cada usuário.                  | [Contact_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v0.json)                | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v0.md) |
| BasicDataSet_v0.Contact_v1         | Contém informações de contato do catálogo de endereços de cada usuário.                        | [Contact_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Contact_v1.json)                | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Contact_v1.md) |
| BasicDataSet_v0.DirectReport_v0    | Contém informações de usuário sobre funcionários que se reportam diretamente a cada usuário.   | [DirectReport_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.DirectReport_v0.json)      | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DirectReport_v0.md) |
| BasicDataSet_v0.Event_v0           | Contém as informações de eventos de calendário de um usuário.                            | [Event_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v0.json)                    | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v0.md) |
| BasicDataSet_v0.Event_v1           | Contém os eventos do calendário de cada usuário.                                       | [Event_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Event_v1.json)                    | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Event_v1.md) |
| BasicDataSet_v0. Inbox_v1      | Contém as pastas de email da caixa de entrada de cada usuário.                                | [Inbox_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Inbox_v1.json)          | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Inbox_v1.md) |
| BasicDataSet_v0.MailboxSettings_v0 | Contém as configurações da caixa de correio de cada usuário.                                        | [MailboxSetting_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailboxSettings_v0.json) | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailboxSettings_v0.md) |
| BasicDataSet_v0.MailFolder_v0      | Contém as pastas de email da caixa de correio de cada usuário.                                | [MailFolder_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.MailFolder_v0.json)          | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/MailFolder_v0.md) |
| BasicDataSet_v0.Manager_v0         | Contém as informações de usuário para o gerenciador de cada usuário.                            | [Manager_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Manager_v0.json)                | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Manager_v0.md) |
| BasicDataSet_v0.Message_v0         | Contém as mensagens de email da caixa de correio de um usuário.                                       | [Message_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v0.json)                | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v0.md) |
| BasicDataSet_v0.Message_v1         | Contém a mensagem de email na caixa de correio de cada usuário.                                       | [Message_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.Message_v1.json)                | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/Message_v1.md) |
| BasicDataSet_v0.SentItem_v0        | Contém as mensagens enviadas da caixa de correio de cada usuário.                               | [SentItem_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v0.json)              | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v0.md) |
| BasicDataSet_v0.SentItem_v1        | Contém a mensagem enviada da caixa de correio de cada usuário.                                | [SentItem_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.SentItem_v1.json)              | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/SentItem_v1.md) |
| BasicDataSet_v0.TeamChat_v1        | Contém [Mensagens de chat do Teams](https://support.microsoft.com/office/first-things-to-know-about-chat-in-microsoft-teams-88ed0a06-6b59-43a3-8cf7-40c01f2f92f2) para mensagens de chat individuais e em grupo. Este conjunto de dados exclui mensagens de chat explicitamente excluídas pelos usuários.     | [TeamChat_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.TeamChat_v1.json)              | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/TeamChat_v1.md) |
| BasicDataSet_v0.User_v0            | Contém informações do usuário (DisplayName, UserPrincipalName e outras informações). | [User_v0](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v0.json)                      | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v0.md) |
| BasicDataSet_v0.User_v1            | Contém informações do usuário.                                                         | [User_v1](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/BasicDataSet_v0.User_v1.json)                      | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/User_v1.md) |
| DocumentSharingDataset_v0_Preview            | Contém informações sobre o compartilhamento de permissões de documentos.                                                         | [DocumentSharingDataset_v0_Preview](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/sampledatasets/DocumentSharingDataset_v0_Preview.json)                      | [Esquema](https://github.com/microsoftgraph/dataconnect-solutions/blob/main/datasetschemas/DocumentSharingDataset_v0_Preview.md) |

## <a name="regions"></a>Regiões

A Conexão de Dados do Microsoft Graph dá suporte à extração de dados de diversas regiões do Microsoft 365. Para mover os dados do datacenter do Microsoft 365 com êxito no armazenamento do seu Microsoft Azure, a instância do Azure Data Factory e o local de armazenamento do Azure devem mapear em uma região com suporte no local dos dados do Microsoft 365. 

A tabela a seguir indica quais regiões do Microsoft 365 têm suporte e as regiões do Azure correspondentes necessárias para a movimentação de dados.

| Região do Office      | Região do Azure                                                   |
| ------------------ | ---------------------------------------------------------------|
| **Ásia – Pacífico**   | <ul><li>Leste da Ásia</li><li>Sudeste da Ásia</li></ul>             |
| **Austrália**      | <ul><li>Leste da Austrália</li><li>Sudeste da Austrália</li></ul>   |
| **Europa**         | <ul><li>Norte da Europa</li><li>Europa Ocidental</li></ul>             |
| **América do Norte**  | <ul><li>EUA Central</li><li>Leste dos EUA</li><li>Leste 2 dos EUA</li><li>Centro-Norte dos EUA</li><li>Centro-Sul dos EUA</li><li>Centro-Oeste dos EUA</li><li>Oeste dos EUA</li><li>Oeste 2 dos EUA</li></ul>                                            |
| **Reino Unido** | <ul><li>Sul do Reino Unido</li><li>Oeste do Reino Unido do Reino Unido</li></ul>                     |

## <a name="sinks"></a>Coletores

Os coletores são os locais da saída que o Azure Data Factory utiliza para colocar dados no armazenamento do Azure. A Conexão de Dados é compatível agora com os seguintes tipos de coletores:

- [Azure Data Lake Storage Gen1](/azure/data-lake-store/data-lake-store-overview)
- [Azure Data Lake Storage Gen2](/azure/storage/blobs/data-lake-storage-introduction)
- [Azure Storage Blob](/azure/storage/blobs/storage-blobs-overview)

Os coletores possuem as seguintes características:

- Os arquivos de saída são do formato de linhas JSON. O formato da saída é fixo e não tem suporte para a modificação do formato da saída. No entanto, você pode usar o Azure Data Factory para copiar o resultado de um pipeline de Conexão de Dados em outro mecanismo de armazenamento (como o Banco de Dados SQL do Azure).
- A autenticação da Entidade de Serviço é o único mecanismo de autenticação com suporte para todos os tipos de coletores em uma atividade de cópia com o Microsoft 365 como a origem.
- Ao usar o Armazenamento de Blob do Azure como coletor, certifique-se de que o aplicativo tem acesso de Colaborador de Dados de Armazenamento de Blob para o local de Armazenamento de Blob do Azure.

## <a name="see-also"></a>Confira também

- [Conector do Azure Data Factory para dados do Microsoft 365](/azure/data-factory/connector-office-365)
- [Políticas e cobrança](data-connect-policies.md)
