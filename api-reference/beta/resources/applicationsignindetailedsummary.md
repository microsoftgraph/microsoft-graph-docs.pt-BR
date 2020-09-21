---
title: tipo de recurso applicationSignInDetailedSummary-API do Microsoft Graph
description: Representa um resumo detalhado de uma entrada de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fca314d1d3f830572a84407ec6c5cb0a28d188d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050241"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>tipo de recurso applicationSignInDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo detalhado de uma entrada de aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Leia as propriedades e os relacionamentos de um objeto **applicationSignInDetailedSummary** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|appDisplayName|Cadeia de caracteres|Nome do aplicativo no qual o usuário entrou.|
|appId|Cadeia de caracteres|ID do aplicativo no qual o usuário entrou.|
|id|Cadeia de caracteres| Uma ID exclusiva que representa a atividade de entrada.|
|signInCount|Int64|Contagem de entradas feitas pelo aplicativo.|
|status|[signInStatus](signinstatus.md)|Detalhes do status de entrada.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


