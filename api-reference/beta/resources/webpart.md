---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510236"
---
# <a name="webpart-resource"></a><span data-ttu-id="24aec-102">recurso de Web Part</span><span class="sxs-lookup"><span data-stu-id="24aec-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24aec-103">O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="24aec-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="24aec-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24aec-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="24aec-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24aec-105">Properties</span></span>

| <span data-ttu-id="24aec-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24aec-106">Property</span></span>                | <span data-ttu-id="24aec-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="24aec-107">Type</span></span>             | <span data-ttu-id="24aec-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="24aec-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="24aec-109">**type**</span><span class="sxs-lookup"><span data-stu-id="24aec-109">**type**</span></span>                | <span data-ttu-id="24aec-110">String</span><span class="sxs-lookup"><span data-stu-id="24aec-110">String</span></span>           | <span data-ttu-id="24aec-111">Um identificador exclusivo especificando o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="24aec-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="24aec-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="24aec-112">Read-only.</span></span>
| <span data-ttu-id="24aec-113">**data**</span><span class="sxs-lookup"><span data-stu-id="24aec-113">**data**</span></span>                | <span data-ttu-id="24aec-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="24aec-114">[sitePageData][]</span></span> | <span data-ttu-id="24aec-115">As propriedades necessárias para a Web Part (varia de acordo com a Web Part)</span><span class="sxs-lookup"><span data-stu-id="24aec-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="24aec-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="24aec-117">Remarks</span></span>

<span data-ttu-id="24aec-118">Web parts do podem definir suas próprias propriedades necessárias em **dados**.</span><span class="sxs-lookup"><span data-stu-id="24aec-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="24aec-119">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="24aec-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
