---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: Web Part
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9147d434a94380c4d178efdf80ccba90734bf96f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939039"
---
# <a name="webpart-resource"></a><span data-ttu-id="995de-102">recurso de Web Part</span><span class="sxs-lookup"><span data-stu-id="995de-102">webPart resource</span></span>

> <span data-ttu-id="995de-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="995de-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="995de-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="995de-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="995de-105">O recurso de **Web Part** representa o tipo e informações de renderização de uma web part em um [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="995de-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="995de-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="995de-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="995de-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="995de-107">Properties</span></span>

| <span data-ttu-id="995de-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="995de-108">Property</span></span>                | <span data-ttu-id="995de-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="995de-109">Type</span></span>             | <span data-ttu-id="995de-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="995de-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="995de-111">**type**</span><span class="sxs-lookup"><span data-stu-id="995de-111">**type**</span></span>                | <span data-ttu-id="995de-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="995de-112">String</span></span>           | <span data-ttu-id="995de-113">Um identificador exclusivo especificando o tipo de Web Part.</span><span class="sxs-lookup"><span data-stu-id="995de-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="995de-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="995de-114">Read-only.</span></span>
| <span data-ttu-id="995de-115">**data**</span><span class="sxs-lookup"><span data-stu-id="995de-115">**data**</span></span>                | <span data-ttu-id="995de-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="995de-116">[sitePageData][]</span></span> | <span data-ttu-id="995de-117">As propriedades necessárias para a Web Part (varia de acordo com a Web Part)</span><span class="sxs-lookup"><span data-stu-id="995de-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="995de-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="995de-119">Remarks</span></span>

<span data-ttu-id="995de-120">Web parts do podem definir suas próprias propriedades necessárias em **dados**.</span><span class="sxs-lookup"><span data-stu-id="995de-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="995de-121">Para obter mais informações sobre páginas, consulte [sitePage](sitepage.md).</span><span class="sxs-lookup"><span data-stu-id="995de-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
