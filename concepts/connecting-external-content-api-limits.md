---
title: Limites de API de conectores do Microsoft Graph
description: A implementação e os limites operacionais dos conectores do Microsoft Graph.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 9e05d022b9bcf2359bdd2a84e8d5707d55c086b6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205617"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Limites de API de conectores do Microsoft Graph

Este artigo descreve a implementação e os limites operacionais dos conectores do Microsoft Graph. Lembre-se desses limites ao criar conectores.

## <a name="connection-limits"></a>Limites de conexão

| **Limite** | **Descrição** |
| --------- | --------------- |
| **10 conexões** | O número máximo de recursos de [conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) por locatário do Microsoft 365. |
| **700.000 itens** | O número máximo de [itens](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) por conexão. |
| **70 GB** | O tamanho máximo de byte de uma conexão. |

## <a name="schema-limits"></a>Limites do esquema

| **Limite** | **Descrição** |
| --------- | --------------- |
| **128 propriedades** | O número máximo de propriedades que podem ser definidas em um [esquema](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true), caracterizando o uso dos dados por meio de uma conexão. |

## <a name="group-limits"></a>Limites de grupo

| **Limite** | **Descrição** |
| --------- | --------------- |
| 100.000 | O número máximo de [grupos externos](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) por locatário do Microsoft 365. |
| **Mil solicitações/seg.** | O número máximo de solicitações permitidas por segundo na [limitação](#throttling) da administração de grupo. |

## <a name="item-ingestion"></a>Ingestão de item

| **Limite** | **Descrição** |
| --------- | --------------- |
| **4 itens/seg (250 MB/hora)** | O limite de produtividade para ingerir itens por meio de uma conexão. |
| **4 MB** | O tamanho máximo de um item; esse limite se aplica ao corpo da solicitação quando [como ingerir e indexar um item](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0). |
| **N/D** | O tamanho máximo de uma propriedade. |

## <a name="throttling"></a>Limitação

Quando um limite da [limitação](throttling.md) é excedido, o Microsoft Graph limita quaisquer outras solicitações desse cliente por um período de tempo. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (Muitas solicitações) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha.

O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de limiar variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.
