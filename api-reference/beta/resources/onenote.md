---
title: tipo de recurso do OneNote
description: O ponto de entrada para recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561646"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="e23ca-103">tipo de recurso do OneNote</span><span class="sxs-lookup"><span data-stu-id="e23ca-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e23ca-104">O ponto de entrada para recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e23ca-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="e23ca-105">Todas as chamadas para o serviço do OneNote por meio da API do Microsoft Graph usam esta URL raiz do serviço:</span><span class="sxs-lookup"><span data-stu-id="e23ca-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="e23ca-106">O local pode ser blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, nos blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="e23ca-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="e23ca-107">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="e23ca-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="e23ca-108">**Blocos de anotações de grupo** Para acessar blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="e23ca-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="e23ca-109">**Blocos de anotações do site do SharePoint** Para acessar blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="e23ca-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="e23ca-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="e23ca-110">Authorization</span></span>

<span data-ttu-id="e23ca-111">Para obter informações sobre as permissões necessárias para trabalhar com as APIs do OneNote, consulte [observações sobre permissões](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e23ca-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="e23ca-112">Relações</span><span class="sxs-lookup"><span data-stu-id="e23ca-112">Relationships</span></span>
| <span data-ttu-id="e23ca-113">Relação</span><span class="sxs-lookup"><span data-stu-id="e23ca-113">Relationship</span></span> | <span data-ttu-id="e23ca-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="e23ca-114">Type</span></span>   |<span data-ttu-id="e23ca-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23ca-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e23ca-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="e23ca-116">notebooks</span></span>|<span data-ttu-id="e23ca-117">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="e23ca-118">O conjunto de blocos de anotações do OneNote pertencentes ao usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e23ca-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="e23ca-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-119">Read-only.</span></span> <span data-ttu-id="e23ca-120">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-120">Nullable.</span></span>|
|<span data-ttu-id="e23ca-121">operations</span><span class="sxs-lookup"><span data-stu-id="e23ca-121">operations</span></span>|<span data-ttu-id="e23ca-122">Coleção [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="e23ca-123">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e23ca-123">The status of OneNote operations.</span></span> <span data-ttu-id="e23ca-124">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status de operações de `Operation-Location` longa duração se o cabeçalho for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e23ca-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="e23ca-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-125">Read-only.</span></span> <span data-ttu-id="e23ca-126">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-126">Nullable.</span></span>|
|<span data-ttu-id="e23ca-127">páginas</span><span class="sxs-lookup"><span data-stu-id="e23ca-127">pages</span></span>|<span data-ttu-id="e23ca-128">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-128">[Page](page.md) collection</span></span>|<span data-ttu-id="e23ca-129">As páginas de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e23ca-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="e23ca-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-130">Read-only.</span></span> <span data-ttu-id="e23ca-131">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-131">Nullable.</span></span>|
|<span data-ttu-id="e23ca-132">recursos</span><span class="sxs-lookup"><span data-stu-id="e23ca-132">resources</span></span>|<span data-ttu-id="e23ca-133">Coleção de [recursos](resource.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="e23ca-134">A imagem e outros recursos de arquivo nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e23ca-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="e23ca-135">Não há suporte para a obtenção de uma coleção Resources, mas você pode [obter o conteúdo binário de um recurso específico](resource.md).</span><span class="sxs-lookup"><span data-stu-id="e23ca-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="e23ca-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-136">Read-only.</span></span> <span data-ttu-id="e23ca-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-137">Nullable.</span></span>|
|<span data-ttu-id="e23ca-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e23ca-138">sectionGroups</span></span>|<span data-ttu-id="e23ca-139">Coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e23ca-140">Os grupos de seções de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e23ca-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="e23ca-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-141">Read-only.</span></span> <span data-ttu-id="e23ca-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-142">Nullable.</span></span>|
|<span data-ttu-id="e23ca-143">sections</span><span class="sxs-lookup"><span data-stu-id="e23ca-143">sections</span></span>|<span data-ttu-id="e23ca-144">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-144">[Section](section.md) collection</span></span>|<span data-ttu-id="e23ca-145">As seções de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.</span><span class="sxs-lookup"><span data-stu-id="e23ca-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="e23ca-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e23ca-146">Read-only.</span></span> <span data-ttu-id="e23ca-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e23ca-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e23ca-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="e23ca-148">Methods</span></span>

| <span data-ttu-id="e23ca-149">Método</span><span class="sxs-lookup"><span data-stu-id="e23ca-149">Method</span></span>           | <span data-ttu-id="e23ca-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e23ca-150">Return Type</span></span>    |<span data-ttu-id="e23ca-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23ca-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e23ca-152">Criar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="e23ca-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="e23ca-153">Bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="e23ca-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="e23ca-154">Crie um bloco de anotações postando na coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="e23ca-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="e23ca-155">Listar blocos de anotações</span><span class="sxs-lookup"><span data-stu-id="e23ca-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="e23ca-156">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="e23ca-157">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="e23ca-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="e23ca-158">Criar página</span><span class="sxs-lookup"><span data-stu-id="e23ca-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="e23ca-159">Page</span><span class="sxs-lookup"><span data-stu-id="e23ca-159">Page</span></span>](page.md)| <span data-ttu-id="e23ca-160">Crie uma página postando na coleção Pages.</span><span class="sxs-lookup"><span data-stu-id="e23ca-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="e23ca-161">Listar páginas</span><span class="sxs-lookup"><span data-stu-id="e23ca-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="e23ca-162">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-162">[Page](page.md) collection</span></span>| <span data-ttu-id="e23ca-163">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="e23ca-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="e23ca-164">Listar grupos de seções</span><span class="sxs-lookup"><span data-stu-id="e23ca-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="e23ca-165">Coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e23ca-166">Obter uma coleção de grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="e23ca-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="e23ca-167">Listar seções</span><span class="sxs-lookup"><span data-stu-id="e23ca-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="e23ca-168">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="e23ca-168">[Section](section.md) collection</span></span>| <span data-ttu-id="e23ca-169">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="e23ca-169">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
