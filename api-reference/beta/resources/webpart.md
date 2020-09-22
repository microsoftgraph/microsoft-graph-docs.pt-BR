---
author: rahmit
description: O recurso webPart representa informações sobre o tipo e a renderização de uma Web Part em um sitePage.
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b69762298f4f165ac18e4e0137dd979bde176652
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973468"
---
# <a name="webpart-resource"></a><span data-ttu-id="1469a-103">recurso webPart</span><span class="sxs-lookup"><span data-stu-id="1469a-103">webPart resource</span></span>

<span data-ttu-id="1469a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1469a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1469a-105">O recurso **WebPart** representa informações sobre o tipo e a renderização de uma Web Part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="1469a-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="1469a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1469a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1469a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1469a-107">Properties</span></span>

| <span data-ttu-id="1469a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1469a-108">Property</span></span>                | <span data-ttu-id="1469a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1469a-109">Type</span></span>             | <span data-ttu-id="1469a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1469a-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="1469a-111">**type**</span><span class="sxs-lookup"><span data-stu-id="1469a-111">**type**</span></span>                | <span data-ttu-id="1469a-112">String</span><span class="sxs-lookup"><span data-stu-id="1469a-112">String</span></span>           | <span data-ttu-id="1469a-113">Um identificador exclusivo que especifica o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="1469a-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="1469a-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1469a-114">Read-only.</span></span>
| <span data-ttu-id="1469a-115">**data**</span><span class="sxs-lookup"><span data-stu-id="1469a-115">**data**</span></span>                | <span data-ttu-id="1469a-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="1469a-116">[sitePageData][]</span></span> | <span data-ttu-id="1469a-117">As propriedades necessárias para a Web Part (varia por webPart)</span><span class="sxs-lookup"><span data-stu-id="1469a-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="1469a-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="1469a-119">Remarks</span></span>

<span data-ttu-id="1469a-120">As Web Parts podem definir suas próprias propriedades obrigatórias em **Data**.</span><span class="sxs-lookup"><span data-stu-id="1469a-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="1469a-121">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="1469a-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
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


