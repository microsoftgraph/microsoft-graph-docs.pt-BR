---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 4e342194fbfc3f73c417b988e3a166ef24b52788
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026380"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="1d6f2-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="1d6f2-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="1d6f2-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d6f2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d6f2-106">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="1d6f2-106">Links to open a OneNote notebook.</span></span> <span data-ttu-id="1d6f2-107">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="1d6f2-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1d6f2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d6f2-108">Properties</span></span>
| <span data-ttu-id="1d6f2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d6f2-109">Property</span></span>     | <span data-ttu-id="1d6f2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d6f2-110">Type</span></span>   |<span data-ttu-id="1d6f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d6f2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d6f2-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="1d6f2-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="1d6f2-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="1d6f2-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="1d6f2-114">Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="1d6f2-114">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="1d6f2-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="1d6f2-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="1d6f2-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="1d6f2-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="1d6f2-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="1d6f2-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d6f2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d6f2-118">JSON representation</span></span>

<span data-ttu-id="1d6f2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d6f2-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


