---
title: tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de entrada do aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType_
ms.openlocfilehash: d169755679cd60285808c1c93cb31810b1d1939d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013333"
---
# <a name="applicationsigninsummary-resource-type"></a>tipo de recurso applicationSignInSummary

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo de entrada do aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter applicationSignInSummary](../api/applicationsigninsummary-get.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e os relacionamentos de um objeto **applicationSignInSummary** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|String|Nome do aplicativo no qual o usuário entrou.|
|appId|String|  ID do aplicativo que o usuário assinou me .\n\nPara.|
|failedSignInCount|Int64|Contagem de entradas com falha feitas pelo aplicativo.|
|successPercentage|Int32|Porcentagem de entradas bem-sucedidas feitas pelo aplicativo.|
|successfulSignInCount|Int64|Contagem de entradas bem-sucedidas feitas pelo aplicativo.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
