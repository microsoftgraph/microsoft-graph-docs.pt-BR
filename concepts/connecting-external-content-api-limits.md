---
title: Limites de API de conectores do Microsoft Graph
description: A implementação e os limites operacionais dos conectores do Microsoft Graph.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: e50085b8c59e304c852f8f75c326fca2967a54f9
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296462"
---
# <a name="microsoft-graph-connectors-api-limits"></a>Limites de API de conectores do Microsoft Graph

Este artigo descreve a implementação e os limites operacionais dos conectores do Microsoft Graph. Lembre-se desses limites ao criar conectores.

## <a name="connection-limits"></a>Limites de conexão

| Tipo de limite | Limite |
| ---------- | ----- |
| Recursos de [Conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-1.0&preserve-view=true) por locatário do Microsoft 365 | 10 |
| [Itens](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true) por conexão | 700.000 |
| Tamanho do byte de conexão | 70 GB |

## <a name="schema-limits"></a>Limites do esquema

| Tipo de limite | Limite |
| ---------- | ----- |
| Propriedades que podem ser definidas em um [esquema](/graph/api/resources/externalconnectors-schema?view=graph-rest-1.0&preserve-view=true), caracterizando os dados ingeridos através de uma conexão | 128 |

## <a name="group-limits"></a>Limites de grupo

| Tipo de limite | Limite |
| ---------- | ----- |
| [Grupos externos](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) por locatário do Microsoft 365 | 100.000 | 
| Solicitações permitidas por segundo (solicitações/s) na administração do grupo [ limitando ](#throttling) limite | 1.000 |

## <a name="item-ingestion"></a>Ingestão de item

| Tipo de limite | Limite |
| ---------- | ----- |
| Limite de taxa de transferência para ingerir itens por meio de uma conexão | 4 itens/s <br> (250 MB/hora) |
| Tamanho do artigo; esse limite se aplica ao [corpo da solicitação ao ingerir e indexar um item](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0) | 4 MB |
| Tamanho da propriedade | N/D |

## <a name="throttling"></a>Limitação

Quando um limite da [limitação](throttling.md) é excedido, o Microsoft Graph limita quaisquer outras solicitações desse cliente por um período de tempo. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (Muitas solicitações) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha.

O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitações serão limitadas. Os limites de controle variam de acordo com o tipo de solicitação. Portanto, você pode encontrar um cenário em que as gravações são limitadas, mas as leituras ainda são permitidas.
