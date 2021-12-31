---
title: Tipo de recurso applicationSignInDetailedSummary
description: Representa um resumo de login do aplicativo.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1c0f07f40ee2b03dd350ea918dc0b1fe43a1b1c5
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647138"
---
# <a name="applicationsigninsummary-resource-type"></a>Tipo de recurso applicationSignInSummary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um resumo de login do aplicativo.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Leia as propriedades e as relações de **um objeto applicationSignInSummary.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|appDisplayName|String|Nome do aplicativo em que o usuário entrou.|
|failedSignInCount|Int64|Contagem de sign-ins com falha feitas pelo aplicativo.|
|successPercentage|Int32|Porcentagem de logins bem-sucedidos feitos pelo aplicativo.|
|successfulSignInCount|Int64|Contagem de logins bem-sucedidos feitos pelo aplicativo.|
<!--Hiding this because it's not in the metadata nor in public response objects
|appId|String|  Identifier of the application that the user signed into.|
-->

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


