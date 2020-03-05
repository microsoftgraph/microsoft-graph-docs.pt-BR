---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 207d7ce3f5cf572d3c32de23882e04a8cc9dd54d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447322"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="c9dd9-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="c9dd9-103">onenote resource type</span></span>

<span data-ttu-id="c9dd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9dd9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9dd9-105">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="c9dd9-106">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c9dd9-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c9dd9-107">A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-107">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="c9dd9-108">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="c9dd9-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="c9dd9-109">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c9dd9-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="c9dd9-110">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c9dd9-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="c9dd9-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9dd9-111">Authorization</span></span>

<span data-ttu-id="c9dd9-112">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="c9dd9-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="c9dd9-113">Relações</span><span class="sxs-lookup"><span data-stu-id="c9dd9-113">Relationships</span></span>
| <span data-ttu-id="c9dd9-114">Relação</span><span class="sxs-lookup"><span data-stu-id="c9dd9-114">Relationship</span></span> | <span data-ttu-id="c9dd9-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9dd9-115">Type</span></span>   |<span data-ttu-id="c9dd9-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9dd9-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9dd9-117">notebooks</span><span class="sxs-lookup"><span data-stu-id="c9dd9-117">notebooks</span></span>|<span data-ttu-id="c9dd9-118">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-118">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="c9dd9-119">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="c9dd9-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-120">Read-only.</span></span> <span data-ttu-id="c9dd9-121">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-121">Nullable.</span></span>|
|<span data-ttu-id="c9dd9-122">operations</span><span class="sxs-lookup"><span data-stu-id="c9dd9-122">operations</span></span>|<span data-ttu-id="c9dd9-123">Coleção [OnenoteOperation](onenoteoperation.md) </span><span class="sxs-lookup"><span data-stu-id="c9dd9-123">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="c9dd9-124">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-124">The status of OneNote operations.</span></span> <span data-ttu-id="c9dd9-125">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="c9dd9-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-126">Read-only.</span></span> <span data-ttu-id="c9dd9-127">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-127">Nullable.</span></span>|
|<span data-ttu-id="c9dd9-128">páginas</span><span class="sxs-lookup"><span data-stu-id="c9dd9-128">pages</span></span>|<span data-ttu-id="c9dd9-129">Coleção [OnenotePage](page.md) </span><span class="sxs-lookup"><span data-stu-id="c9dd9-129">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="c9dd9-130">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c9dd9-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-131">Read-only.</span></span> <span data-ttu-id="c9dd9-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-132">Nullable.</span></span>|
|<span data-ttu-id="c9dd9-133">recursos</span><span class="sxs-lookup"><span data-stu-id="c9dd9-133">resources</span></span>|<span data-ttu-id="c9dd9-134">Coleção [OnenoteResource](resource.md) </span><span class="sxs-lookup"><span data-stu-id="c9dd9-134">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="c9dd9-135">A imagem e outros recursos de arquivos nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="c9dd9-136">Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md).</span><span class="sxs-lookup"><span data-stu-id="c9dd9-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="c9dd9-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-137">Read-only.</span></span> <span data-ttu-id="c9dd9-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-138">Nullable.</span></span>|
|<span data-ttu-id="c9dd9-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="c9dd9-139">sectionGroups</span></span>|<span data-ttu-id="c9dd9-140">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-140">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="c9dd9-141">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c9dd9-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-142">Read-only.</span></span> <span data-ttu-id="c9dd9-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-143">Nullable.</span></span>|
|<span data-ttu-id="c9dd9-144">seções</span><span class="sxs-lookup"><span data-stu-id="c9dd9-144">sections</span></span>|<span data-ttu-id="c9dd9-145">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-145">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="c9dd9-146">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c9dd9-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-147">Read-only.</span></span> <span data-ttu-id="c9dd9-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="c9dd9-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9dd9-149">Methods</span></span>

| <span data-ttu-id="c9dd9-150">Método</span><span class="sxs-lookup"><span data-stu-id="c9dd9-150">Method</span></span>           | <span data-ttu-id="c9dd9-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9dd9-151">Return Type</span></span>    |<span data-ttu-id="c9dd9-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9dd9-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9dd9-153">Create notebook</span><span class="sxs-lookup"><span data-stu-id="c9dd9-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="c9dd9-154">Notebook</span><span class="sxs-lookup"><span data-stu-id="c9dd9-154">Notebook</span></span>](notebook.md)| <span data-ttu-id="c9dd9-155">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="c9dd9-156">List notebooks</span><span class="sxs-lookup"><span data-stu-id="c9dd9-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="c9dd9-157">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-157">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="c9dd9-158">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="c9dd9-159">Create page</span><span class="sxs-lookup"><span data-stu-id="c9dd9-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="c9dd9-160">Page</span><span class="sxs-lookup"><span data-stu-id="c9dd9-160">Page</span></span>](page.md)| <span data-ttu-id="c9dd9-161">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="c9dd9-162">List pages</span><span class="sxs-lookup"><span data-stu-id="c9dd9-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="c9dd9-163">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-163">[Page](page.md) collection</span></span>| <span data-ttu-id="c9dd9-164">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="c9dd9-165">List section groups</span><span class="sxs-lookup"><span data-stu-id="c9dd9-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="c9dd9-166">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-166">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="c9dd9-167">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="c9dd9-168">Listar seções</span><span class="sxs-lookup"><span data-stu-id="c9dd9-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="c9dd9-169">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="c9dd9-169">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="c9dd9-170">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-170">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="c9dd9-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9dd9-171">JSON Representation</span></span>
<span data-ttu-id="c9dd9-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9dd9-172">Here is a JSON representation of the resource.</span></span>
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
