---
title: Tipo de recurso autoReviewSettings
description: Especifica o comportamento de quando uma revisão de acesso é concluída.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f46ef4b57a921cc08fbb8f3768597eef12c1ce4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136928"
---
# <a name="autoreviewsettings-resource-type"></a>Tipo de recurso autoReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **tipo de recurso autoReviewSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica o comportamento de quando uma revisão de acesso é concluída.    

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| notReviewedResult | String | Valores possíveis: `Approve` `Deny` , ou `Recommendation` .  If `Recommendation` , then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true` . Se você quiser que o sistema forneça uma decisão mesmo se o revisor não fizer uma escolha, defina a propriedade **autoReviewEnabled** no recurso **accessReviewSettings** para e inclua um objeto `true` **autoReviewSettings** com a propriedade **notReviewedResult.** Em seguida, quando uma revisão é concluída, com base na **propriedade notReviewedResult,** a decisão é registrada como `Approve` um ou `Deny` .|

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
