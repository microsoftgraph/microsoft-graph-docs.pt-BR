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
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="d0501-103">tipo de recurso autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d0501-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="d0501-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0501-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0501-105">O tipo de recurso **autoReviewSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica o comportamento de quando uma revisão do Access é concluída.</span><span class="sxs-lookup"><span data-stu-id="d0501-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="d0501-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0501-106">Properties</span></span>

| <span data-ttu-id="d0501-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0501-107">Property</span></span> | <span data-ttu-id="d0501-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0501-108">Type</span></span> | <span data-ttu-id="d0501-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0501-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="d0501-110">notReviewedResult</span><span class="sxs-lookup"><span data-stu-id="d0501-110">notReviewedResult</span></span> | <span data-ttu-id="d0501-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d0501-111">String</span></span> | <span data-ttu-id="d0501-112">Valores possíveis: `Approve` , `Deny` , ou `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="d0501-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="d0501-113">Se `Recommendation` , em seguida, **accessRecommendationsEnabled** no recurso **accessReviewSettings** também deverá ser definido como `true` .</span><span class="sxs-lookup"><span data-stu-id="d0501-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="d0501-114">Se você deseja que o sistema ofereça uma decisão mesmo se o revisor não fizer uma escolha, defina a propriedade **autoReviewEnabled** no recurso **accessReviewSettings** para `true` e inclua um objeto **autoReviewSettings** com a propriedade **notReviewedResult** .</span><span class="sxs-lookup"><span data-stu-id="d0501-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="d0501-115">Em seguida, quando uma revisão é concluída, com base na propriedade **notReviewedResult** , a decisão é registrada como `Approve` ou `Deny` .</span><span class="sxs-lookup"><span data-stu-id="d0501-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0501-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0501-116">JSON representation</span></span>

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