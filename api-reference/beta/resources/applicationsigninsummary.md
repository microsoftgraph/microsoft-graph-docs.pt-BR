---
title: tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de entrada do aplicativo.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0e654df6af359069bbc476c5419a20ca0429f9a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050238"
---
# <a name="applicationsigninsummary-resource-type"></a>tipo de recurso applicationSignInSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo de entrada do aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter applicationSignInSummary](../api/applicationsigninsummary-get.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e os relacionamentos de um objeto **applicationSignInSummary** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|Cadeia de caracteres|Nome do aplicativo no qual o usuário entrou.|
|appId|Cadeia de caracteres|  ID do aplicativo que o usuário assinou me .\n\nPara.|
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


