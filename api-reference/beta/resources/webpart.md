---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e7bbd0f6aa8d4ea04304d6aecae97b98ab0a46b7
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574275"
---
# <a name="webpart-resource"></a><span data-ttu-id="cc3d6-102">recurso de Web Part</span><span class="sxs-lookup"><span data-stu-id="cc3d6-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc3d6-103">O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="cc3d6-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc3d6-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc3d6-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  
    ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "String (identifier)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="cc3d6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc3d6-105">Properties</span></span>

| <span data-ttu-id="cc3d6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc3d6-106">Property</span></span>                | <span data-ttu-id="cc3d6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc3d6-107">Type</span></span>             | <span data-ttu-id="cc3d6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc3d6-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="cc3d6-109">**type**</span><span class="sxs-lookup"><span data-stu-id="cc3d6-109">**type**</span></span>                | <span data-ttu-id="cc3d6-110">Cadeia de caracteres (identificador)</span><span class="sxs-lookup"><span data-stu-id="cc3d6-110">String (identifier)</span></span>         | <span data-ttu-id="cc3d6-111">Um identificador exclusivo especificando o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="cc3d6-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-112">Read-only.</span></span>
| <span data-ttu-id="cc3d6-113">**data**</span><span class="sxs-lookup"><span data-stu-id="cc3d6-113">**data**</span></span>                | [<span data-ttu-id="cc3d6-114">sitePageData</span><span class="sxs-lookup"><span data-stu-id="cc3d6-114">sitePageData</span></span>](sitepagedata.md) | <span data-ttu-id="cc3d6-115">As propriedades necessárias para a Web Part (varia de acordo com a Web Part)</span><span class="sxs-lookup"><span data-stu-id="cc3d6-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="cc3d6-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="cc3d6-116">Remarks</span></span>

<span data-ttu-id="cc3d6-117">Web parts do podem definir suas próprias propriedades necessárias em **dados**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-117">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="cc3d6-118">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="cc3d6-118">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
