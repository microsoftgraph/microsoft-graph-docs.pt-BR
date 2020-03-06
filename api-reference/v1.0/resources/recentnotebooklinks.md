---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4eefb69476af9769795198fc7e67b154fa30eb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533895"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="d98aa-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="d98aa-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="d98aa-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d98aa-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d98aa-106">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="d98aa-106">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="d98aa-107">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="d98aa-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d98aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d98aa-108">Properties</span></span>
| <span data-ttu-id="d98aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d98aa-109">Property</span></span>     | <span data-ttu-id="d98aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d98aa-110">Type</span></span>   |<span data-ttu-id="d98aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d98aa-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d98aa-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="d98aa-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="d98aa-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="d98aa-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="d98aa-114">Abre o bloco de anotações no cliente nativo do OneNote se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="d98aa-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="d98aa-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="d98aa-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="d98aa-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="d98aa-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="d98aa-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="d98aa-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d98aa-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d98aa-118">JSON representation</span></span>

<span data-ttu-id="d98aa-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d98aa-119">The following is a JSON representation of the resource.</span></span>

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
