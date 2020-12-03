---
title: tipo de recurso signInStatus
description: Fornece o status de entrada (sucesso ou falha) da entrada
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3633968869c0cf61e16afa4ba056a530c86b3c93
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563650"
---
# <a name="signinstatus-resource-type"></a>tipo de recurso signInStatus

Namespace: microsoft.graph

Fornece o status de entrada (sucesso ou falha) da entrada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalDetails|String|Fornece detalhes adicionais sobre a atividade de entrada|
|errorCode|Int32|Fornece o código de erro de dígito 5-6 gerado durante uma falha de entrada. Confira a [lista de códigos e mensagens de erro](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).|
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

