---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 4114704a13b4116534d96743ceacfba51df67847
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812442"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="b401d-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="b401d-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="b401d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b401d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b401d-106">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="b401d-106">Links to open a OneNote notebook.</span></span> <span data-ttu-id="b401d-107">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="b401d-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b401d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b401d-108">Properties</span></span>
| <span data-ttu-id="b401d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b401d-109">Property</span></span>     | <span data-ttu-id="b401d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b401d-110">Type</span></span>   |<span data-ttu-id="b401d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b401d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b401d-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="b401d-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="b401d-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="b401d-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="b401d-114">Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="b401d-114">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="b401d-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="b401d-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="b401d-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="b401d-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="b401d-117">Abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="b401d-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b401d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b401d-118">JSON representation</span></span>

<span data-ttu-id="b401d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b401d-119">The following is a JSON representation of the resource.</span></span>

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
