---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453606"
---
# <a name="webpart-resource"></a><span data-ttu-id="163f9-102">recurso webPart</span><span class="sxs-lookup"><span data-stu-id="163f9-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="163f9-103">O recurso **WebPart** representa informações sobre o tipo e a renderização de uma Web Part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="163f9-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="163f9-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="163f9-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="163f9-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="163f9-105">Properties</span></span>

| <span data-ttu-id="163f9-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="163f9-106">Property</span></span>                | <span data-ttu-id="163f9-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="163f9-107">Type</span></span>             | <span data-ttu-id="163f9-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="163f9-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="163f9-109">**type**</span><span class="sxs-lookup"><span data-stu-id="163f9-109">**type**</span></span>                | <span data-ttu-id="163f9-110">String</span><span class="sxs-lookup"><span data-stu-id="163f9-110">String</span></span>           | <span data-ttu-id="163f9-111">Um identificador exclusivo que especifica o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="163f9-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="163f9-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="163f9-112">Read-only.</span></span>
| <span data-ttu-id="163f9-113">**data**</span><span class="sxs-lookup"><span data-stu-id="163f9-113">**data**</span></span>                | <span data-ttu-id="163f9-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="163f9-114">[sitePageData][]</span></span> | <span data-ttu-id="163f9-115">As propriedades necessárias para a Web Part (varia por webPart)</span><span class="sxs-lookup"><span data-stu-id="163f9-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="163f9-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="163f9-117">Remarks</span></span>

<span data-ttu-id="163f9-118">As Web Parts podem definir suas próprias propriedades obrigatórias em **Data**.</span><span class="sxs-lookup"><span data-stu-id="163f9-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="163f9-119">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="163f9-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
