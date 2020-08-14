---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 72adb53bdf50ee0a5c909b54cb11698fc593f8db
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2020
ms.locfileid: "46657914"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="5212d-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="5212d-103">onenote resource type</span></span>

<span data-ttu-id="5212d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5212d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5212d-105">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5212d-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="5212d-106">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="5212d-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="5212d-107">O local pode ser os blocos de notas do usuário no Microsoft 365 ou no OneDrive do consumidor, blocos de notas do grupo ou blocos de notas de equipe hospedados no site do SharePoint no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5212d-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="5212d-108">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="5212d-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="5212d-109">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="5212d-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="5212d-110">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="5212d-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="5212d-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="5212d-111">Authorization</span></span>

<span data-ttu-id="5212d-112">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="5212d-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="5212d-113">Relações</span><span class="sxs-lookup"><span data-stu-id="5212d-113">Relationships</span></span>
| <span data-ttu-id="5212d-114">Relação</span><span class="sxs-lookup"><span data-stu-id="5212d-114">Relationship</span></span> | <span data-ttu-id="5212d-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="5212d-115">Type</span></span>   |<span data-ttu-id="5212d-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5212d-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5212d-117">notebooks</span><span class="sxs-lookup"><span data-stu-id="5212d-117">notebooks</span></span>|<span data-ttu-id="5212d-118">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-118">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="5212d-119">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="5212d-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="5212d-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-120">Read-only.</span></span> <span data-ttu-id="5212d-121">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-121">Nullable.</span></span>|
|<span data-ttu-id="5212d-122">operations</span><span class="sxs-lookup"><span data-stu-id="5212d-122">operations</span></span>|<span data-ttu-id="5212d-123">Coleção [OnenoteOperation](onenoteoperation.md) </span><span class="sxs-lookup"><span data-stu-id="5212d-123">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="5212d-124">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5212d-124">The status of OneNote operations.</span></span> <span data-ttu-id="5212d-125">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="5212d-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="5212d-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-126">Read-only.</span></span> <span data-ttu-id="5212d-127">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-127">Nullable.</span></span>|
|<span data-ttu-id="5212d-128">páginas</span><span class="sxs-lookup"><span data-stu-id="5212d-128">pages</span></span>|<span data-ttu-id="5212d-129">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="5212d-129">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="5212d-130">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="5212d-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="5212d-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-131">Read-only.</span></span> <span data-ttu-id="5212d-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-132">Nullable.</span></span>|
|<span data-ttu-id="5212d-133">recursos</span><span class="sxs-lookup"><span data-stu-id="5212d-133">resources</span></span>|<span data-ttu-id="5212d-134">Coleção [OnenoteResource](resource.md) </span><span class="sxs-lookup"><span data-stu-id="5212d-134">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="5212d-135">A imagem e outros recursos de arquivos nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="5212d-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="5212d-136">Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md).</span><span class="sxs-lookup"><span data-stu-id="5212d-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="5212d-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-137">Read-only.</span></span> <span data-ttu-id="5212d-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-138">Nullable.</span></span>|
|<span data-ttu-id="5212d-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="5212d-139">sectionGroups</span></span>|<span data-ttu-id="5212d-140">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-140">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="5212d-141">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="5212d-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="5212d-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-142">Read-only.</span></span> <span data-ttu-id="5212d-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-143">Nullable.</span></span>|
|<span data-ttu-id="5212d-144">seções</span><span class="sxs-lookup"><span data-stu-id="5212d-144">sections</span></span>|<span data-ttu-id="5212d-145">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-145">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="5212d-146">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="5212d-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="5212d-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5212d-147">Read-only.</span></span> <span data-ttu-id="5212d-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="5212d-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="5212d-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="5212d-149">Methods</span></span>

| <span data-ttu-id="5212d-150">Método</span><span class="sxs-lookup"><span data-stu-id="5212d-150">Method</span></span>           | <span data-ttu-id="5212d-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5212d-151">Return Type</span></span>    |<span data-ttu-id="5212d-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="5212d-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5212d-153">Create notebook</span><span class="sxs-lookup"><span data-stu-id="5212d-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="5212d-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="5212d-154">Notebook</span></span>](notebook.md)| <span data-ttu-id="5212d-155">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="5212d-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="5212d-156">List notebooks</span><span class="sxs-lookup"><span data-stu-id="5212d-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="5212d-157">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-157">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="5212d-158">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="5212d-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="5212d-159">Create page</span><span class="sxs-lookup"><span data-stu-id="5212d-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="5212d-160">Page</span><span class="sxs-lookup"><span data-stu-id="5212d-160">Page</span></span>](page.md)| <span data-ttu-id="5212d-161">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="5212d-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="5212d-162">List pages</span><span class="sxs-lookup"><span data-stu-id="5212d-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="5212d-163">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-163">[Page](page.md) collection</span></span>| <span data-ttu-id="5212d-164">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="5212d-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="5212d-165">List section groups</span><span class="sxs-lookup"><span data-stu-id="5212d-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="5212d-166">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-166">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="5212d-167">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="5212d-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="5212d-168">Listar seções</span><span class="sxs-lookup"><span data-stu-id="5212d-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="5212d-169">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="5212d-169">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="5212d-170">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="5212d-170">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="5212d-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5212d-171">JSON Representation</span></span>
<span data-ttu-id="5212d-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5212d-172">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
```json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
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
