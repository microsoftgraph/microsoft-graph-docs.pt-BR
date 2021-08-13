---
title: Tipo de recurso userFeedback
description: O tipo userFeedback.
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4f38484219f33432aa5f4c215869c5f6df33aba133d38bcc79ce4f52a28eb2c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180884"
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
