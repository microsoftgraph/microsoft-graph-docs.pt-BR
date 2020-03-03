---
title: tipo de recurso userfeedback
description: O tipo userfeedback.
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0ab9c49563bb4715b1736618a939b681178ddae8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394654"
---
# <a name="userfeedback-resource-type"></a>tipo de recurso userfeedback

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os comentários fornecidos pelo usuário para um ponto de extremidade sobre a qualidade da sessão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|classificação|String|A classificação fornecida pelo usuário deste ponto de extremidade sobre a qualidade desta sessão. Os valores possíveis são: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|texto|String|O texto de comentários fornecido pelo usuário deste ponto de extremidade para a sessão.|
|sinais|[Microsoft. Graph. callRecords. feedbackTokenSet](callrecords-feedbacktokenset.md)|O conjunto de tokens de comentários fornecidos pelo usuário deste ponto de extremidade para a sessão. Este é um conjunto de propriedades booleanas. Os nomes de propriedade não devem ser dependentes, já que eles podem ser alterados, dependendo de quais tokens são oferecidos para o usuário.|

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