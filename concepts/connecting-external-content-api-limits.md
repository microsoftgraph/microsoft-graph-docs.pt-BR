---
title: Limites de API de conector do Microsoft Graph
description: Limites de API de conector do Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 6ab757d16a10f2291ad9bac5034e9fe7357a7188
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645672"
---
# <a name="microsoft-graph-connector-api-limits"></a>Limites de API de conector do Microsoft Graph

Este tópico descreve os limites operacionais e de implementação dos conectores do Microsoft Graph. Lembre-se desses limites ao criar conectores.

## <a name="connection-limits"></a>Limites de conexão

| **Limite** | **Descrição** |
| --- | --- |
| **10 conexões** | O número máximo de recursos de [conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) por locatário do Microsoft 365. |
| **700.000 itens** | O número máximo de [itens](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) por conexão. |
| **70 GB** | O tamanho máximo de byte de uma conexão. |

## <a name="schema-limits"></a>Limites do esquema

| **Limite** | **Descrição** |
| --- | --- |
| **128 propriedades** | O número máximo de propriedades que podem ser definidas em um [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), caracterizando o uso dos dados por meio de uma conexão. |

## <a name="group-limits"></a>Limites de grupo

| **Limite** | **Descrição** |
| --- | --- |
| 100.000 | O número máximo de [grupos externos](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) por locatário do Microsoft 365. |
| **Mil solicitações/seg.** | O número máximo de solicitações permitidas por segundo na [limitação](#throttling) da administração de grupo. |

## <a name="item-ingestion"></a>Ingestão de item

| **Limite** | **Descrição** |
| --- | --- |
| **4 itens/seg (250 MB/hora)** | O limite de produtividade para ingerir itens por meio de uma conexão. |
| **4 MB** | O tamanho máximo de um item; esse limite se aplica ao corpo da solicitação quando [como ingerir e indexar um item](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true). |
| **N/D** | O tamanho máximo de uma propriedade. |

## <a name="throttling"></a>Limitação

Quando a restrição do [limite](throttling.md) for excedida, o Microsoft Graph limita quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.
