---
title: tipo de recurso de signInStatus
description: Fornece o status de entrada (sucesso ou falha) do sign-in
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878635"
---
# <a name="signinstatus-resource-type"></a>tipo de recurso de signInStatus
Fornece o status de entrada (sucesso ou falha) do sign-in



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|Cadeia de caracteres|Fornece detalhes adicionais sobre a atividade de entrada|
|errorCode|Int32|Fornece o código de erro 5-6digit gerado durante uma falha de entrada. Confira a [lista de mensagens e códigos de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|Cadeia de caracteres|Fornece a mensagem de erro ou o motivo da falha da atividade de entrada correspondente. Confira a [lista de mensagens e códigos de erro](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

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
