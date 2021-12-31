---
title: Tipo de recurso applicationSignInDetailedSummary - API Graph Microsoft
description: Representa um resumo detalhado de uma assinatura de aplicativo.
ms.localizationpriority: medium
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b929e35904af0ddec506a8b1b47e502456adb3c6
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647166"
---
# <a name="applicationsignindetailedsummary-resource-type"></a>Tipo de recurso applicationSignInDetailedSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo detalhado de uma assinatura de aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [Coleção applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Recuperar **objetos applicationSignInDetailedSummary.** |
| [Obter applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Leia as propriedades e as relações de um **objeto applicationSignInDetailedSummary.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|aggregatedEventDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|appDisplayName|String|Nome do aplicativo ao que o usuário se inscreveu.|
|appId|String|ID do aplicativo ao que o usuário se inscreveu.|
|id|String| Uma ID exclusiva que representa a atividade de login.|
|signInCount|Int64|Contagem de assinaturas feitas pelo aplicativo.|
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


