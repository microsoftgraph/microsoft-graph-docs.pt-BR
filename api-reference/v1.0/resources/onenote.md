---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0311e514c7d15e8b5fafcc94beecaecdcc6d9d49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035851"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="ef661-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="ef661-103">onenote resource type</span></span>

<span data-ttu-id="ef661-104">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ef661-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="ef661-105">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="ef661-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="ef661-106">A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="ef661-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="ef661-107">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="ef661-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="ef661-108">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="ef661-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="ef661-109">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="ef661-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="ef661-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef661-110">Authorization</span></span>

<span data-ttu-id="ef661-111">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="ef661-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="ef661-112">Relações</span><span class="sxs-lookup"><span data-stu-id="ef661-112">Relationships</span></span>
| <span data-ttu-id="ef661-113">Relação</span><span class="sxs-lookup"><span data-stu-id="ef661-113">Relationship</span></span> | <span data-ttu-id="ef661-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef661-114">Type</span></span>   |<span data-ttu-id="ef661-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef661-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef661-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="ef661-116">notebooks</span></span>|<span data-ttu-id="ef661-117">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="ef661-118">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="ef661-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="ef661-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-119">Read-only.</span></span> <span data-ttu-id="ef661-120">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-120">Nullable.</span></span>|
|<span data-ttu-id="ef661-121">operations</span><span class="sxs-lookup"><span data-stu-id="ef661-121">operations</span></span>|<span data-ttu-id="ef661-122">Coleção [OnenoteOperation](onenoteoperation.md) </span><span class="sxs-lookup"><span data-stu-id="ef661-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="ef661-123">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ef661-123">The status of OneNote operations.</span></span> <span data-ttu-id="ef661-124">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="ef661-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="ef661-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-125">Read-only.</span></span> <span data-ttu-id="ef661-126">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-126">Nullable.</span></span>|
|<span data-ttu-id="ef661-127">páginas</span><span class="sxs-lookup"><span data-stu-id="ef661-127">pages</span></span>|<span data-ttu-id="ef661-128">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="ef661-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="ef661-129">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="ef661-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ef661-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-130">Read-only.</span></span> <span data-ttu-id="ef661-131">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-131">Nullable.</span></span>|
|<span data-ttu-id="ef661-132">recursos</span><span class="sxs-lookup"><span data-stu-id="ef661-132">resources</span></span>|<span data-ttu-id="ef661-133">Coleção [OnenoteResource](resource.md) </span><span class="sxs-lookup"><span data-stu-id="ef661-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="ef661-134">A imagem e outros recursos de arquivos nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="ef661-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="ef661-135">Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md).</span><span class="sxs-lookup"><span data-stu-id="ef661-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="ef661-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-136">Read-only.</span></span> <span data-ttu-id="ef661-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-137">Nullable.</span></span>|
|<span data-ttu-id="ef661-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="ef661-138">sectionGroups</span></span>|<span data-ttu-id="ef661-139">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="ef661-140">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="ef661-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ef661-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-141">Read-only.</span></span> <span data-ttu-id="ef661-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-142">Nullable.</span></span>|
|<span data-ttu-id="ef661-143">seções</span><span class="sxs-lookup"><span data-stu-id="ef661-143">sections</span></span>|<span data-ttu-id="ef661-144">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="ef661-145">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="ef661-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="ef661-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef661-146">Read-only.</span></span> <span data-ttu-id="ef661-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef661-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="ef661-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="ef661-148">Methods</span></span>

| <span data-ttu-id="ef661-149">Método</span><span class="sxs-lookup"><span data-stu-id="ef661-149">Method</span></span>           | <span data-ttu-id="ef661-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ef661-150">Return Type</span></span>    |<span data-ttu-id="ef661-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef661-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ef661-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="ef661-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="ef661-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="ef661-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="ef661-154">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="ef661-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="ef661-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="ef661-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="ef661-156">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="ef661-157">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="ef661-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="ef661-158">Create page</span><span class="sxs-lookup"><span data-stu-id="ef661-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="ef661-159">Page</span><span class="sxs-lookup"><span data-stu-id="ef661-159">Page</span></span>](page.md)| <span data-ttu-id="ef661-160">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="ef661-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="ef661-161">List pages</span><span class="sxs-lookup"><span data-stu-id="ef661-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="ef661-162">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-162">[Page](page.md) collection</span></span>| <span data-ttu-id="ef661-163">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="ef661-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="ef661-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="ef661-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="ef661-165">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="ef661-166">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="ef661-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="ef661-167">Listar seções</span><span class="sxs-lookup"><span data-stu-id="ef661-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="ef661-168">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="ef661-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="ef661-169">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="ef661-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ef661-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef661-170">JSON Representation</span></span>
<span data-ttu-id="ef661-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ef661-171">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
