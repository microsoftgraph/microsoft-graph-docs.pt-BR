---
title: Tipo de recurso autoReviewSettings (preterido)
description: Especifica o comportamento de quando uma revisão de acesso é concluída.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 593c07266432a389b0f63891675fa9f4823db784
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820256"
---
# <a name="autoreviewsettings-resource-type-deprecated"></a>Tipo de recurso autoReviewSettings (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

O **tipo de recurso autoReviewSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica o comportamento de quando uma revisão de acesso é concluída.    

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| notReviewedResult | Cadeia de caracteres | Valores possíveis: `Approve`, `Deny`ou `Recommendation`.  If `Recommendation`, **então accessRecommendationsEnabled** no **recurso accessReviewSettings** também deve ser definido como `true`. Se você quiser que o sistema forneça uma decisão mesmo que o revisor não faça uma escolha, defina a propriedade **autoReviewEnabled** no recurso **accessReviewSettings** `true` para e inclua um **objeto autoReviewSettings** com a propriedade **notReviewedResult** . Em seguida, quando uma revisão é concluída, com base na **propriedade notReviewedResult** , a decisão é registrada como um ou `Approve` `Deny`.|

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.autoReviewSettings"
}-->
```json
{
  "notReviewedResult": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "autoReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
