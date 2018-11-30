---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036140"
---
# <a name="webpart-resource"></a><span data-ttu-id="da847-102">recurso de Web Part</span><span class="sxs-lookup"><span data-stu-id="da847-102">webPart resource</span></span>

> <span data-ttu-id="da847-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da847-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da847-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da847-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da847-105">O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="da847-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="da847-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da847-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="da847-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da847-107">Properties</span></span>

| <span data-ttu-id="da847-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da847-108">Property</span></span>                | <span data-ttu-id="da847-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da847-109">Type</span></span>             | <span data-ttu-id="da847-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da847-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="da847-111">**type**</span><span class="sxs-lookup"><span data-stu-id="da847-111">**type**</span></span>                | <span data-ttu-id="da847-112">String</span><span class="sxs-lookup"><span data-stu-id="da847-112">String</span></span>           | <span data-ttu-id="da847-113">Um identificador exclusivo especificando o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="da847-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="da847-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da847-114">Read-only.</span></span>
| <span data-ttu-id="da847-115">**data**</span><span class="sxs-lookup"><span data-stu-id="da847-115">**data**</span></span>                | <span data-ttu-id="da847-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="da847-116">[sitePageData][]</span></span> | <span data-ttu-id="da847-117">As propriedades necessárias para a Web Part (varia de acordo com a Web Part)</span><span class="sxs-lookup"><span data-stu-id="da847-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="da847-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="da847-119">Remarks</span></span>

<span data-ttu-id="da847-120">Web parts do podem definir suas próprias propriedades necessárias em **dados**.</span><span class="sxs-lookup"><span data-stu-id="da847-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="da847-121">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="da847-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
