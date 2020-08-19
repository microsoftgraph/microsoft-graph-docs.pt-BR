---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fb828db87a5e883933a8cac72cf99f50c4bdd480
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806846"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="9fdf1-104">tipo de recurso recentNotebook</span><span class="sxs-lookup"><span data-stu-id="9fdf1-104">recentNotebook resource type</span></span>

<span data-ttu-id="9fdf1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fdf1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fdf1-106">Um bloco de notas do OneNote recentemente acessado.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-106">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="9fdf1-107">Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-107">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="9fdf1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fdf1-108">Properties</span></span>
| <span data-ttu-id="9fdf1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fdf1-109">Property</span></span>     | <span data-ttu-id="9fdf1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fdf1-110">Type</span></span>   |<span data-ttu-id="9fdf1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fdf1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9fdf1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9fdf1-112">displayName</span></span>|<span data-ttu-id="9fdf1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fdf1-113">String</span></span>|<span data-ttu-id="9fdf1-114">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-114">The name of the notebook.</span></span>|
|<span data-ttu-id="9fdf1-115">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="9fdf1-115">lastAccessedTime</span></span>|<span data-ttu-id="9fdf1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fdf1-116">DateTimeOffset</span></span>|<span data-ttu-id="9fdf1-117">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-117">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="9fdf1-118">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fdf1-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9fdf1-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-120">Read-only.</span></span>|
|<span data-ttu-id="9fdf1-121">links</span><span class="sxs-lookup"><span data-stu-id="9fdf1-121">links</span></span>|[<span data-ttu-id="9fdf1-122">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="9fdf1-122">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="9fdf1-123">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-123">Links for opening the notebook.</span></span> <span data-ttu-id="9fdf1-124">O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-124">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="9fdf1-125">O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-125">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="9fdf1-126">sourceService</span><span class="sxs-lookup"><span data-stu-id="9fdf1-126">sourceService</span></span>|<span data-ttu-id="9fdf1-127">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="9fdf1-127">onenoteSourceService</span></span>|<span data-ttu-id="9fdf1-128">A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-128">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9fdf1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fdf1-129">JSON representation</span></span>

<span data-ttu-id="9fdf1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="9fdf1-131">Métodos</span><span class="sxs-lookup"><span data-stu-id="9fdf1-131">Methods</span></span>

| <span data-ttu-id="9fdf1-132">Método</span><span class="sxs-lookup"><span data-stu-id="9fdf1-132">Method</span></span>           | <span data-ttu-id="9fdf1-133">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9fdf1-133">Return Type</span></span>    |<span data-ttu-id="9fdf1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fdf1-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9fdf1-135">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="9fdf1-135">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="9fdf1-136">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="9fdf1-136">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="9fdf1-137">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9fdf1-137">Get a collection of the most recently accessed notebooks for the user.</span></span> |
