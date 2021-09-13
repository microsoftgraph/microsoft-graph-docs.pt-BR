---
title: Tipo de recurso userFeedback
description: O tipo userFeedback.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 830b279c4021ec08677a4a5ebaf637bc73b7beaf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084661"
---
# <a name="userfeedback-resource-type"></a>Tipo de recurso userFeedback

Namespace: microsoft.graph.callRecords

Representa os comentários fornecidos pelo usuário um ponto de extremidade sobre a qualidade da sessão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|rating|microsoft.graph.callRecords.userFeedbackRating|A classificação fornecida pelo usuário deste ponto de extremidade sobre a qualidade desta Sessão. Os valores possíveis são: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|texto|Cadeia de caracteres|O texto de comentários fornecido pelo usuário deste ponto de extremidade para a sessão.|
|tokens|[microsoft.graph.callRecords.feedbackTokenSet](callrecords-feedbacktokenset.md)|O conjunto de tokens de feedback fornecidos pelo usuário deste ponto de extremidade para a sessão. Este é um conjunto de propriedades Boolean. Os nomes de propriedade não devem ser confiados, pois eles podem mudar dependendo de quais tokens são oferecidos ao usuário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.userFeedback",
  "baseType": null
}-->

```json
{
  "rating": "String",
  "text": "String",
  "tokens": {"@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
