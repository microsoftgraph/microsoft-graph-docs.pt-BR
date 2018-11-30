---
title: Tipo de recurso notebookLinks
description: Links para abrir um bloco de anotações do OneNote.
ms.openlocfilehash: 713779d3bab12222df7a405c1dccb4e6cd4cb235
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005144"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="15f99-103">Tipo de recurso notebookLinks</span><span class="sxs-lookup"><span data-stu-id="15f99-103">notebookLinks resource type</span></span>

<span data-ttu-id="15f99-104">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="15f99-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="15f99-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15f99-105">JSON representation</span></span>

<span data-ttu-id="15f99-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15f99-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="15f99-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15f99-107">Properties</span></span>
| <span data-ttu-id="15f99-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15f99-108">Property</span></span>     | <span data-ttu-id="15f99-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="15f99-109">Type</span></span>   |<span data-ttu-id="15f99-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="15f99-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="15f99-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="15f99-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="15f99-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="15f99-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="15f99-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="15f99-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="15f99-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="15f99-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="15f99-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="15f99-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="15f99-116">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="15f99-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->