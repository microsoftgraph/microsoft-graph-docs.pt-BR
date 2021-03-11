---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: a35553ddb182597f1d5427418283216f962f207c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721731"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="93a22-104">tipo de recurso recentNotebook</span><span class="sxs-lookup"><span data-stu-id="93a22-104">recentNotebook resource type</span></span>

<span data-ttu-id="93a22-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93a22-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a22-106">Um bloco de notas do OneNote recentemente acessado.</span><span class="sxs-lookup"><span data-stu-id="93a22-106">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="93a22-107">Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.</span><span class="sxs-lookup"><span data-stu-id="93a22-107">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="93a22-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93a22-108">Properties</span></span>
| <span data-ttu-id="93a22-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93a22-109">Property</span></span>     | <span data-ttu-id="93a22-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="93a22-110">Type</span></span>   |<span data-ttu-id="93a22-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93a22-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93a22-112">displayName</span><span class="sxs-lookup"><span data-stu-id="93a22-112">displayName</span></span>|<span data-ttu-id="93a22-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93a22-113">String</span></span>|<span data-ttu-id="93a22-114">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="93a22-114">The name of the notebook.</span></span>|
|<span data-ttu-id="93a22-115">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="93a22-115">lastAccessedTime</span></span>|<span data-ttu-id="93a22-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93a22-116">DateTimeOffset</span></span>|<span data-ttu-id="93a22-117">A data e hora da última modificação do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="93a22-117">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="93a22-118">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="93a22-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="93a22-119">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="93a22-119">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="93a22-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93a22-120">Read-only.</span></span>|
|<span data-ttu-id="93a22-121">links</span><span class="sxs-lookup"><span data-stu-id="93a22-121">links</span></span>|[<span data-ttu-id="93a22-122">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="93a22-122">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="93a22-123">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="93a22-123">Links for opening the notebook.</span></span> <span data-ttu-id="93a22-124">O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="93a22-124">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="93a22-125">O `oneNoteWebURL` link abre o bloco de anotações no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="93a22-125">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="93a22-126">sourceService</span><span class="sxs-lookup"><span data-stu-id="93a22-126">sourceService</span></span>|<span data-ttu-id="93a22-127">String</span><span class="sxs-lookup"><span data-stu-id="93a22-127">String</span></span>|<span data-ttu-id="93a22-128">A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.</span><span class="sxs-lookup"><span data-stu-id="93a22-128">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93a22-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93a22-129">JSON representation</span></span>

<span data-ttu-id="93a22-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93a22-130">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="93a22-131">Métodos</span><span class="sxs-lookup"><span data-stu-id="93a22-131">Methods</span></span>

| <span data-ttu-id="93a22-132">Método</span><span class="sxs-lookup"><span data-stu-id="93a22-132">Method</span></span>           | <span data-ttu-id="93a22-133">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="93a22-133">Return Type</span></span>    |<span data-ttu-id="93a22-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="93a22-134">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="93a22-135">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="93a22-135">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="93a22-136">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="93a22-136">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="93a22-137">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="93a22-137">Get a collection of the most recently accessed notebooks for the user.</span></span> |


