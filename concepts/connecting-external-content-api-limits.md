---
title: Limites de API de conectores do Microsoft Graph
description: Tenha em mente a implementação e os limites operacionais ao criar conectores do Microsoft Graph. Inclui limites de conexão, esquema e grupo.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: e21f40d99b2a7d56050fa6e8cf119ece7df259d3
ms.sourcegitcommit: 6a4e81d2b8e7447771c9060998c7e1cc18a57902
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2022
ms.locfileid: "66609637"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Limites de API de conectores do Microsoft Graph

Este artigo descreve a implementação e os limites operacionais dos conectores do Microsoft Graph. Lembre-se desses limites ao criar conectores.

## <a name="connection-limits"></a>Limites de conexão

| Tipo de limite | Limite |
| ---------- | ----- |
| Recursos de [Conexão](/graph/api/resources/externalconnectors-externalconnection) por locatário do Microsoft 365 | 10 para pesquisa, 15 para conformidade |
| [Itens](/graph/api/resources/externalconnectors-externalitem) por conexão | 5,000,000 |
| Tamanho do byte de conexão | 500 GB |

## <a name="schema-limits"></a>Limites do esquema

| Tipo de limite | Limite |
| ---------- | ----- |
| Propriedades que podem ser definidas em um [esquema](/graph/api/resources/externalconnectors-schema), caracterizando os dados ingeridos através de uma conexão | 128 |

## <a name="group-limits"></a>Limites de grupo

| Tipo de limite | Limite |
| ---------- | ----- |
| [Grupos externos](/graph/api/resources/externalconnectors-externalgroup) por locatário do Microsoft 365 | 100.000 | 
| Solicitações permitidas por segundo (solicitações/s) na administração do grupo [ limitando ](#throttling) limite | 1.000 |

## <a name="item-ingestion"></a>Ingestão de item

| Tipo de limite | Limite |
| ---------- | ----- |
| Limite de taxa de transferência para ingerir itens por meio de uma conexão | 25 itens/s |
| Tamanho do artigo; esse limite se aplica ao [corpo da solicitação ao ingerir e indexar um item](/graph/api/externalconnectors-externalconnection-put-items) | 4 MB |
| Tamanho da propriedade | N/D |

## <a name="throttling"></a>Limitação

Quando um limite da [limitação](throttling.md) é excedido, o Microsoft Graph limita quaisquer outras solicitações desse cliente por um período de tempo. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (Muitas solicitações) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha.

O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitações serão limitadas. Os limites de controle variam de acordo com o tipo de solicitação. Portanto, você pode encontrar um cenário em que as gravações são limitadas, mas as leituras ainda são permitidas.
