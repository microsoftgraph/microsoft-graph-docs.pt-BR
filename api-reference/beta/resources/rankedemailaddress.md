---
title: tipo de recurso de rankedEmailAddress
description: Representa um endereço de email classificados.
localization_priority: Normal
ms.openlocfilehash: 938afc0de208fd3cdbd0cfec299d01ada9d4f592
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510005"
---
# <a name="rankedemailaddress-resource-type"></a><span data-ttu-id="3fd9c-103">tipo de recurso de rankedEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3fd9c-103">rankedEmailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fd9c-104">Representa um endereço de email classificados.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-104">Represents a ranked email address.</span></span>


## <a name="properties"></a><span data-ttu-id="3fd9c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fd9c-105">Properties</span></span>
| <span data-ttu-id="3fd9c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fd9c-106">Property</span></span>     | <span data-ttu-id="3fd9c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fd9c-107">Type</span></span>   |<span data-ttu-id="3fd9c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fd9c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3fd9c-109">address</span><span class="sxs-lookup"><span data-stu-id="3fd9c-109">address</span></span>|<span data-ttu-id="3fd9c-110">string</span><span class="sxs-lookup"><span data-stu-id="3fd9c-110">string</span></span>|<span data-ttu-id="3fd9c-111">O endereço de email.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-111">The email address.</span></span>|
|<span data-ttu-id="3fd9c-112">rank</span><span class="sxs-lookup"><span data-stu-id="3fd9c-112">rank</span></span>|<span data-ttu-id="3fd9c-113">double</span><span class="sxs-lookup"><span data-stu-id="3fd9c-113">double</span></span>|<span data-ttu-id="3fd9c-114">A classificação do endereço de email.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-114">The rank of the email address.</span></span> <span data-ttu-id="3fd9c-115">Uma classificação é usada como uma chave de classificação, em relação as outros resultados retornados.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-115">A rank is used as a sort key, in relation to the other returned results.</span></span> <span data-ttu-id="3fd9c-116">Um valor de classificação mais alto corresponde a um resultado mais relevante.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-116">A higher rank value corresponds to a more relevant result.</span></span> <span data-ttu-id="3fd9c-117">A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-117">Relevance is determined by communication, collaboration, and business relationship signals.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3fd9c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fd9c-118">JSON representation</span></span>

<span data-ttu-id="3fd9c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fd9c-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/rankedemailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
