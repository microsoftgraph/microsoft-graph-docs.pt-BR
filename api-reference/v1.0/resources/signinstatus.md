---
title: Tipo de recurso signInStatus
description: Fornece o status de login (Sucesso ou Falha) da assinatura
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 87181dd2ec911d2ebaa613dd4bc7ad4d46182a2d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139580"
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

