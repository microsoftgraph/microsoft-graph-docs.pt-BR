---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 7cb48f7a4235b28231ab93fc3ccfba074f80d286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808596"
---
# <a name="signinstatus-resource-type"></a>tipo de recurso signInStatus

Namespace: o Microsoft. Graph fornece o status de entrada (êxito ou falha) da entrada



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|String|Fornece detalhes adicionais sobre a atividade de entrada|
|errorCode|Int32|Fornece o código de erro de 5 6digit que é gerado durante uma falha de entrada. Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|Cadeia de caracteres|Fornece a mensagem de erro ou o motivo da falha para a atividade de entrada correspondente. Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

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
