---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345781"
---
# <a name="webpart-resource"></a><span data-ttu-id="d9020-102">recurso webPart</span><span class="sxs-lookup"><span data-stu-id="d9020-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9020-103">O recurso **WebPart** representa informações sobre o tipo e a renderização de uma Web Part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="d9020-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9020-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9020-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d9020-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9020-105">Properties</span></span>

| <span data-ttu-id="d9020-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9020-106">Property</span></span>                | <span data-ttu-id="d9020-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9020-107">Type</span></span>             | <span data-ttu-id="d9020-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9020-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="d9020-109">**type**</span><span class="sxs-lookup"><span data-stu-id="d9020-109">**type**</span></span>                | <span data-ttu-id="d9020-110">String</span><span class="sxs-lookup"><span data-stu-id="d9020-110">String</span></span>           | <span data-ttu-id="d9020-111">Um identificador exclusivo que especifica o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="d9020-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="d9020-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9020-112">Read-only.</span></span>
| <span data-ttu-id="d9020-113">**data**</span><span class="sxs-lookup"><span data-stu-id="d9020-113">**data**</span></span>                | <span data-ttu-id="d9020-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="d9020-114">[sitePageData][]</span></span> | <span data-ttu-id="d9020-115">As propriedades necessárias para a Web Part (varia por webPart)</span><span class="sxs-lookup"><span data-stu-id="d9020-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="d9020-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9020-117">Remarks</span></span>

<span data-ttu-id="d9020-118">As Web Parts podem definir suas próprias propriedades obrigatórias em **Data**.</span><span class="sxs-lookup"><span data-stu-id="d9020-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="d9020-119">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="d9020-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
