---
title: Tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 2666d7da98eeb6115a179ddbbadcd8b5e7f941d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826877"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="2b1b4-103">Tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="2b1b4-103">notebookLinks resource type</span></span>

<span data-ttu-id="2b1b4-104">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="2b1b4-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b1b4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b1b4-105">JSON representation</span></span>

<span data-ttu-id="2b1b4-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b1b4-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="2b1b4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b1b4-107">Properties</span></span>
| <span data-ttu-id="2b1b4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b1b4-108">Property</span></span>     | <span data-ttu-id="2b1b4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b1b4-109">Type</span></span>   |<span data-ttu-id="2b1b4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b1b4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b1b4-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="2b1b4-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="2b1b4-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="2b1b4-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="2b1b4-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="2b1b4-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="2b1b4-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="2b1b4-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="2b1b4-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="2b1b4-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="2b1b4-116">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="2b1b4-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
