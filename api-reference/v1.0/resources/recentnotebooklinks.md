---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
ms.openlocfilehash: 594616a790becd77086177157f71321ffdd36e24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004442"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="c194b-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="c194b-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="c194b-105">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c194b-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="c194b-106">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="c194b-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c194b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c194b-107">Properties</span></span>
| <span data-ttu-id="c194b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c194b-108">Property</span></span>     | <span data-ttu-id="c194b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c194b-109">Type</span></span>   |<span data-ttu-id="c194b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c194b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c194b-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="c194b-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="c194b-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="c194b-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="c194b-113">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="c194b-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="c194b-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="c194b-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="c194b-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="c194b-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="c194b-116">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="c194b-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c194b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c194b-117">JSON representation</span></span>

<span data-ttu-id="c194b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c194b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
