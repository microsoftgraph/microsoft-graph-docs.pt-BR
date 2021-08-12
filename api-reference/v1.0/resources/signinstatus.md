---
title: Tipo de recurso signInStatus
description: Fornece o status de login (Sucesso ou Falha) da assinatura
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 350ed66245164b5745d7b6f0bc962ebab5b1b4e46e8d7fc6b9a5c45b17ccc3a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222669"
---
# <a name="signinstatus-resource-type"></a>Tipo de recurso signInStatus

Namespace: microsoft.graph

Fornece o status de login (Êxito ou Falha) da assinatura.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|String|Fornece detalhes adicionais sobre a atividade de login|
|errorCode|Int32|Fornece o código de erro de 5 a 6 dígitos gerado durante uma falha de login. Confira a lista [de códigos de erro e mensagens](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
|failureReason|Cadeia de caracteres|Fornece a mensagem de erro ou o motivo da falha na atividade de login correspondente. Confira a lista [de códigos de erro e mensagens](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|

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

