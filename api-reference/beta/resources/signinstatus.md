---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d336e226b2855687da0aae889afd9d92141c895c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008303"
---
# <a name="signinstatus-resource-type"></a>tipo de recurso signInStatus
Fornece o status de entrada (sucesso ou falha) da entrada



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|String|Fornece detalhes adicionais sobre a atividade de entrada|
|errorCode|Int32|Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada. Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|Cadeia de caracteres|Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente. Confira a [lista de códigos e mensagens de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
