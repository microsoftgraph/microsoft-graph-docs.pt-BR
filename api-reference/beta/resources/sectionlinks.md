---
title: tipo de recurso sectionLinks
description: Links para abrir uma seção do OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 9ee3022ede7da1fbbfa6074611f54590e027209c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087583"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="ed6b0-103">tipo de recurso sectionLinks</span><span class="sxs-lookup"><span data-stu-id="ed6b0-103">sectionLinks resource type</span></span>

<span data-ttu-id="ed6b0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed6b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed6b0-105">Links para abrir uma seção do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ed6b0-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed6b0-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed6b0-106">JSON representation</span></span>

<span data-ttu-id="ed6b0-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed6b0-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ed6b0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed6b0-108">Properties</span></span>
| <span data-ttu-id="ed6b0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed6b0-109">Property</span></span>     | <span data-ttu-id="ed6b0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed6b0-110">Type</span></span>   |<span data-ttu-id="ed6b0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed6b0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed6b0-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ed6b0-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="ed6b0-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed6b0-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed6b0-114">Abre a seção no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="ed6b0-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ed6b0-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ed6b0-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="ed6b0-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="ed6b0-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="ed6b0-117">Abre a seção no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="ed6b0-117">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


