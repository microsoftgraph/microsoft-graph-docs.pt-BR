---
title: tipo de recurso applicationSignInDetailedSummary-API do Microsoft Graph
description: Representa um resumo detalhado de uma entrada de aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 118d26e6d46e5b64861a041eec12d03bea533552
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508272"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>tipo de recurso applicationSignInDetailedSummary

Namespace: Microsoft. Graph

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
|appDisplayName|String|Nome do aplicativo no qual o usuário entrou.|
|appId|String|ID do aplicativo no qual o usuário entrou.|
|id|String| Uma ID exclusiva que representa a atividade de entrada.|
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
