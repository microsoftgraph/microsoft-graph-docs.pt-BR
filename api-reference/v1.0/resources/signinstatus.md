---
title: Tipo de recurso signInStatus
description: Fornece o status de login (Êxito ou Falha) da assinatura
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 37eb91434fd7a5fb0dc65f5c7203effd42f3878e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137085"
---
# <a name="signinstatus-resource-type"></a>Tipo de recurso signInStatus

Namespace: microsoft.graph

Fornece o status de login (Êxito ou Falha) da login.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|String|Fornece detalhes adicionais sobre a atividade de login|
|errorCode|Int32|Fornece o código de erro de 5 a 6 dígitos gerado durante uma falha de login. Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|
|failureReason|Cadeia de caracteres|Fornece a mensagem de erro ou o motivo da falha para a atividade de login correspondente. Confira a lista [de códigos de erro e mensagens.](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)|

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

