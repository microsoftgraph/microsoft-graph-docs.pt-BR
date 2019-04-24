---
title: tipo de recurso site
description: Representa um site da Web.
localization_priority: Normal
ms.openlocfilehash: 3f8aadaf0a6b6beb2394664f04195267062dc9ae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454041"
---
# <a name="website-resource-type"></a><span data-ttu-id="d6382-103">tipo de recurso site</span><span class="sxs-lookup"><span data-stu-id="d6382-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6382-104">Representa um site da Web.</span><span class="sxs-lookup"><span data-stu-id="d6382-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="d6382-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6382-105">Properties</span></span>
| <span data-ttu-id="d6382-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6382-106">Property</span></span>     | <span data-ttu-id="d6382-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6382-107">Type</span></span>   |<span data-ttu-id="d6382-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6382-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6382-109">type</span><span class="sxs-lookup"><span data-stu-id="d6382-109">type</span></span>|<span data-ttu-id="d6382-110">String</span><span class="sxs-lookup"><span data-stu-id="d6382-110">String</span></span>| <span data-ttu-id="d6382-111">Os valores possíveis são: `other`, `home`, `work`, `blog`, `profile`.</span><span class="sxs-lookup"><span data-stu-id="d6382-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="d6382-112">address</span><span class="sxs-lookup"><span data-stu-id="d6382-112">address</span></span>|<span data-ttu-id="d6382-113">string</span><span class="sxs-lookup"><span data-stu-id="d6382-113">string</span></span>|<span data-ttu-id="d6382-114">A URL do site.</span><span class="sxs-lookup"><span data-stu-id="d6382-114">The URL of the website.</span></span>|
|<span data-ttu-id="d6382-115">displayName</span><span class="sxs-lookup"><span data-stu-id="d6382-115">displayName</span></span>|<span data-ttu-id="d6382-116">string</span><span class="sxs-lookup"><span data-stu-id="d6382-116">string</span></span>|<span data-ttu-id="d6382-117">O nome de exibição do site da Web.</span><span class="sxs-lookup"><span data-stu-id="d6382-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6382-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6382-118">JSON representation</span></span>

<span data-ttu-id="d6382-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6382-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/website.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
