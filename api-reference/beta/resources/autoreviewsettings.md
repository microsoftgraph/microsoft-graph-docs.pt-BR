---
title: tipo de recurso autoReviewSettings
description: Especifica o comportamento de quando uma revisão do Access é concluída.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b9d0a621c4229476e0b3bcdadb869e44422e931
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330316"
---
# <a name="autoreviewsettings-resource-type"></a>tipo de recurso autoReviewSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **autoReviewSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica o comportamento de quando uma revisão do Access é concluída.    

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| notReviewedResult | Cadeia de caracteres | Valores possíveis: `Approve` , `Deny` , ou `Recommendation` .  Se `Recommendation` , em seguida, **accessRecommendationsEnabled** no recurso **accessReviewSettings** também deverá ser definido como `true` . Se você deseja que o sistema ofereça uma decisão mesmo se o revisor não fizer uma escolha, defina a propriedade **autoReviewEnabled** no recurso **accessReviewSettings** para `true` e inclua um objeto **autoReviewSettings** com a propriedade **notReviewedResult** . Em seguida, quando uma revisão é concluída, com base na propriedade **notReviewedResult** , a decisão é registrada como `Approve` ou `Deny` .|

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