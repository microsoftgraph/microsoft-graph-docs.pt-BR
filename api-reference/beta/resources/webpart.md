---
author: rahmit
description: O recurso webPart representa informações sobre o tipo e a renderização de uma Web Part em um sitePage.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007351"
---
# <a name="webpart-resource"></a><span data-ttu-id="1df7a-103">recurso webPart</span><span class="sxs-lookup"><span data-stu-id="1df7a-103">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1df7a-104">O recurso **WebPart** representa informações sobre o tipo e a renderização de uma Web Part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="1df7a-104">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1df7a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1df7a-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a><span data-ttu-id="1df7a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1df7a-106">Properties</span></span>

| <span data-ttu-id="1df7a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1df7a-107">Property</span></span>                | <span data-ttu-id="1df7a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1df7a-108">Type</span></span>             | <span data-ttu-id="1df7a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df7a-109">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="1df7a-110">**type**</span><span class="sxs-lookup"><span data-stu-id="1df7a-110">**type**</span></span>                | <span data-ttu-id="1df7a-111">String</span><span class="sxs-lookup"><span data-stu-id="1df7a-111">String</span></span>           | <span data-ttu-id="1df7a-112">Um identificador exclusivo que especifica o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="1df7a-112">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="1df7a-113">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1df7a-113">Read-only.</span></span>
| <span data-ttu-id="1df7a-114">**data**</span><span class="sxs-lookup"><span data-stu-id="1df7a-114">**data**</span></span>                | <span data-ttu-id="1df7a-115">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="1df7a-115">[sitePageData][]</span></span> | <span data-ttu-id="1df7a-116">As propriedades necessárias para a Web Part (varia por webPart)</span><span class="sxs-lookup"><span data-stu-id="1df7a-116">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="1df7a-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="1df7a-118">Remarks</span></span>

<span data-ttu-id="1df7a-119">As Web Parts podem definir suas próprias propriedades obrigatórias em **Data**.</span><span class="sxs-lookup"><span data-stu-id="1df7a-119">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="1df7a-120">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="1df7a-120">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
