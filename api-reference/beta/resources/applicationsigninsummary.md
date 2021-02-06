---
title: Tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de login do aplicativo.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 454c4e2e9e57b61194e6f3e6970e5db1ea414369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137407"
---
# <a name="applicationsigninsummary-resource-type"></a>Tipo de recurso applicationSignInSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo de login do aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter applicationSignInSummary](../api/applicationsigninsummary-get.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e os relacionamentos de **um objeto applicationSignInSummary.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|String|Nome do aplicativo em que o usuário se inscreveu.|
|appId|String|  ID do aplicativo que o usuário assinou i nto.|
|failedSignInCount|Int64|Contagem de falhas de logins feitas pelo aplicativo.|
|successPercentage|Int32|Porcentagem de logins bem-sucedidos feitos pelo aplicativo.|
|successfulSignInCount|Int64|Contagem de logins bem-sucedidos feitos pelo aplicativo.|

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


