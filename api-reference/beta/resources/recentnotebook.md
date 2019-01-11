---
title: tipo de recurso recentNotebook
description: Um bloco de notas do OneNote recentemente acessado. Um **recentNotebook** é similar a um notebook, mas tem menos propriedades.
localization_priority: Normal
ms.openlocfilehash: f2dd1ca642203cde36bb636b9cb2eb7c79344e3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833828"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="351be-104">tipo de recurso recentNotebook</span><span class="sxs-lookup"><span data-stu-id="351be-104">recentNotebook resource type</span></span>

> <span data-ttu-id="351be-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="351be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="351be-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="351be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="351be-107">Um bloco de notas do OneNote recentemente acessado.</span><span class="sxs-lookup"><span data-stu-id="351be-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="351be-108">Um **recentNotebook** é similar a um [notebook](notebook.md), mas tem menos propriedades.</span><span class="sxs-lookup"><span data-stu-id="351be-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="351be-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="351be-109">Properties</span></span>
| <span data-ttu-id="351be-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="351be-110">Property</span></span>     | <span data-ttu-id="351be-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="351be-111">Type</span></span>   |<span data-ttu-id="351be-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="351be-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="351be-113">name</span><span class="sxs-lookup"><span data-stu-id="351be-113">name</span></span>|<span data-ttu-id="351be-114">String</span><span class="sxs-lookup"><span data-stu-id="351be-114">String</span></span>|<span data-ttu-id="351be-115">O nome do bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="351be-115">The name of the notebook.</span></span>|
|<span data-ttu-id="351be-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="351be-116">lastAccessedTime</span></span>|<span data-ttu-id="351be-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="351be-117">DateTimeOffset</span></span>|<span data-ttu-id="351be-p104">A data e hora da última modificação do bloco de anotações. O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="351be-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="351be-122">links</span><span class="sxs-lookup"><span data-stu-id="351be-122">links</span></span>|[<span data-ttu-id="351be-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="351be-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="351be-124">Links para abrir o bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="351be-124">Links for opening the notebook.</span></span> <span data-ttu-id="351be-125">O link `oneNoteClientURL` abre o bloco de anotações no cliente do OneNote quando ele está instalado.</span><span class="sxs-lookup"><span data-stu-id="351be-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="351be-126">O link `oneNoteWebURL` abre o bloco de anotações no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="351be-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="351be-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="351be-127">sourceService</span></span>|<span data-ttu-id="351be-128">String</span><span class="sxs-lookup"><span data-stu-id="351be-128">String</span></span>|<span data-ttu-id="351be-129">A loja de back-end onde o bloco de anotações (notebook) reside, tanto em `OneDriveForBusiness` ou em `OneDrive`.</span><span class="sxs-lookup"><span data-stu-id="351be-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="351be-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="351be-130">JSON representation</span></span>

<span data-ttu-id="351be-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="351be-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="351be-132">Métodos</span><span class="sxs-lookup"><span data-stu-id="351be-132">Methods</span></span>

| <span data-ttu-id="351be-133">Método</span><span class="sxs-lookup"><span data-stu-id="351be-133">Method</span></span>           | <span data-ttu-id="351be-134">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="351be-134">Return Type</span></span>    |<span data-ttu-id="351be-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="351be-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="351be-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="351be-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="351be-137">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="351be-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="351be-138">Obtenha uma coleção de blocos de anotações acessados mais recentemente para o usuário.</span><span class="sxs-lookup"><span data-stu-id="351be-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
