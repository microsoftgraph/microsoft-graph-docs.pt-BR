---
title: tipo de recurso recentNotebookLinks
description: Links para abrir um bloco de anotações do OneNote. Esse tipo de recurso existe como uma propriedade em um recurso recentNotebook.
ms.openlocfilehash: de13f25148425a1816a60f6cf5b9f4a09f61c7dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036726"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="98376-104">tipo de recurso recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="98376-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="98376-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="98376-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98376-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98376-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98376-107">Links para abrir um bloco de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="98376-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="98376-108">Esse tipo de recurso existe como uma propriedade em um recurso [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="98376-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="98376-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98376-109">Properties</span></span>
| <span data-ttu-id="98376-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98376-110">Property</span></span>     | <span data-ttu-id="98376-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="98376-111">Type</span></span>   |<span data-ttu-id="98376-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="98376-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98376-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="98376-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="98376-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="98376-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="98376-115">Abre o bloco de anotações no cliente do OneNote, se ele estiver instalado.</span><span class="sxs-lookup"><span data-stu-id="98376-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="98376-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="98376-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="98376-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="98376-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="98376-118">Abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="98376-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98376-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98376-119">JSON representation</span></span>

<span data-ttu-id="98376-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98376-120">The following is a JSON representation of the resource.</span></span>

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
