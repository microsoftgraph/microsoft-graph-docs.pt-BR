---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6961a267948c62ac1d24623c6d8bbeaf94f7569
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078994"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="e600c-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="e600c-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="e600c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e600c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e600c-106">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e600c-106">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="e600c-107">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="e600c-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e600c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e600c-108">Properties</span></span>
| <span data-ttu-id="e600c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e600c-109">Property</span></span>     | <span data-ttu-id="e600c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e600c-110">Type</span></span>   |<span data-ttu-id="e600c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e600c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e600c-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e600c-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="e600c-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="e600c-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="e600c-114">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="e600c-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="e600c-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e600c-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="e600c-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="e600c-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="e600c-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="e600c-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e600c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e600c-118">JSON representation</span></span>

<span data-ttu-id="e600c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e600c-119">The following is a JSON representation of the resource.</span></span>

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

