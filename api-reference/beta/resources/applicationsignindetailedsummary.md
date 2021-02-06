---
title: Tipo de recurso applicationSignInDetailedSummary - API do Microsoft Graph
description: Representa um resumo detalhado de uma inscrição de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: d0d1eaa15d71dfa219271cef74880a092e9522db
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137442"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>Tipo de recurso applicationSignInDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo detalhado de uma inscrição de aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Leia as propriedades e os relacionamentos de **um objeto applicationSignInDetailedSummary.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|appDisplayName|String|Nome do aplicativo em que o usuário se inscreveu.|
|appId|String|ID do aplicativo em que o usuário se inscreveu.|
|id|String| Uma ID exclusiva que representa a atividade de login.|
|signInCount|Int64|Contagem de sign-ins feitas pelo aplicativo.|
|status|[signInStatus](signinstatus.md)|Detalhes do status de login.|

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


