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
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="d2936-103">Tipo de recurso autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="d2936-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="d2936-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2936-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2936-105">O **tipo de recurso autoReviewSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica o comportamento de quando uma revisão de acesso é concluída.</span><span class="sxs-lookup"><span data-stu-id="d2936-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="d2936-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2936-106">Properties</span></span>

| <span data-ttu-id="d2936-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2936-107">Property</span></span> | <span data-ttu-id="d2936-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2936-108">Type</span></span> | <span data-ttu-id="d2936-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2936-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="d2936-110">notReviewedResult</span><span class="sxs-lookup"><span data-stu-id="d2936-110">notReviewedResult</span></span> | <span data-ttu-id="d2936-111">String</span><span class="sxs-lookup"><span data-stu-id="d2936-111">String</span></span> | <span data-ttu-id="d2936-112">Valores possíveis: `Approve` `Deny` , ou `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="d2936-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="d2936-113">If `Recommendation` , then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true` .</span><span class="sxs-lookup"><span data-stu-id="d2936-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="d2936-114">Se você quiser que o sistema forneça uma decisão mesmo se o revisor não fizer uma escolha, defina a propriedade **autoReviewEnabled** no recurso **accessReviewSettings** para e inclua um objeto `true` **autoReviewSettings** com a propriedade **notReviewedResult.**</span><span class="sxs-lookup"><span data-stu-id="d2936-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="d2936-115">Em seguida, quando uma revisão é concluída, com base na **propriedade notReviewedResult,** a decisão é registrada como `Approve` um ou `Deny` .</span><span class="sxs-lookup"><span data-stu-id="d2936-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2936-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2936-116">JSON representation</span></span>

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
