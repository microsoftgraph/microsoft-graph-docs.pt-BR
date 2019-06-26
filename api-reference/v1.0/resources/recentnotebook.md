---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
ms.openlocfilehash: fb5e7a7b75ea62bc644d19cf895666ba106d5dd9
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236654"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="dc8cb-104">tipo de recurso recentNotebook</span><span class="sxs-lookup"><span data-stu-id="dc8cb-104">recentNotebook resource type</span></span>

<span data-ttu-id="dc8cb-105">Um bloco de notas do OneNote recentemente acessado.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="dc8cb-106">Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="dc8cb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc8cb-107">Properties</span></span>
| <span data-ttu-id="dc8cb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc8cb-108">Property</span></span>     | <span data-ttu-id="dc8cb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc8cb-109">Type</span></span>   |<span data-ttu-id="dc8cb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc8cb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc8cb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="dc8cb-111">displayName</span></span>|<span data-ttu-id="dc8cb-112">String</span><span class="sxs-lookup"><span data-stu-id="dc8cb-112">String</span></span>|<span data-ttu-id="dc8cb-113">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-113">The name of the notebook.</span></span>|
|<span data-ttu-id="dc8cb-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="dc8cb-114">lastAccessedTime</span></span>|<span data-ttu-id="dc8cb-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc8cb-115">DateTimeOffset</span></span>|<span data-ttu-id="dc8cb-116">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-116">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="dc8cb-117">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dc8cb-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="dc8cb-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-119">Read-only.</span></span>|
|<span data-ttu-id="dc8cb-120">links</span><span class="sxs-lookup"><span data-stu-id="dc8cb-120">links</span></span>|[<span data-ttu-id="dc8cb-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="dc8cb-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="dc8cb-122">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-122">Links for opening the notebook.</span></span> <span data-ttu-id="dc8cb-123">O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="dc8cb-124">O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-124">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="dc8cb-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="dc8cb-125">sourceService</span></span>|<span data-ttu-id="dc8cb-126">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="dc8cb-126">onenoteSourceService</span></span>|<span data-ttu-id="dc8cb-127">A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc8cb-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc8cb-128">JSON representation</span></span>

<span data-ttu-id="dc8cb-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}
```

## <a name="methods"></a><span data-ttu-id="dc8cb-130">Métodos</span><span class="sxs-lookup"><span data-stu-id="dc8cb-130">Methods</span></span>

| <span data-ttu-id="dc8cb-131">Método</span><span class="sxs-lookup"><span data-stu-id="dc8cb-131">Method</span></span>           | <span data-ttu-id="dc8cb-132">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dc8cb-132">Return Type</span></span>    |<span data-ttu-id="dc8cb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc8cb-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dc8cb-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="dc8cb-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="dc8cb-135">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="dc8cb-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="dc8cb-136">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
