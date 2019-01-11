---
title: Tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839932"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="145cf-103">Tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="145cf-103">sectionLinks resource type</span></span>

<span data-ttu-id="145cf-104">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="145cf-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="145cf-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="145cf-105">JSON representation</span></span>

<span data-ttu-id="145cf-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="145cf-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="145cf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="145cf-107">Properties</span></span>
| <span data-ttu-id="145cf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="145cf-108">Property</span></span>     | <span data-ttu-id="145cf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="145cf-109">Type</span></span>   |<span data-ttu-id="145cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="145cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="145cf-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="145cf-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="145cf-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="145cf-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="145cf-113">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="145cf-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="145cf-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="145cf-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="145cf-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="145cf-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="145cf-116">Abre a seção no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="145cf-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
