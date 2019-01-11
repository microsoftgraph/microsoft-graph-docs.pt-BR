---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 5ccf861541526a1673d6174176cb8b2a62df6c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812870"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="e71a9-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="e71a9-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="e71a9-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e71a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e71a9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e71a9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e71a9-107">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e71a9-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="e71a9-108">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="e71a9-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="e71a9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e71a9-109">Properties</span></span>
| <span data-ttu-id="e71a9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e71a9-110">Property</span></span>     | <span data-ttu-id="e71a9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e71a9-111">Type</span></span>   |<span data-ttu-id="e71a9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e71a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e71a9-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="e71a9-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="e71a9-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="e71a9-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="e71a9-115">Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="e71a9-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="e71a9-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="e71a9-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="e71a9-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="e71a9-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="e71a9-118">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="e71a9-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e71a9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e71a9-119">JSON representation</span></span>

<span data-ttu-id="e71a9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e71a9-120">The following is a JSON representation of the resource.</span></span>

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
