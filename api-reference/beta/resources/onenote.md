---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 1fe12502832c6fb6053488989f95838e8dc77adb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039220"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="bc970-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="bc970-103">onenote resource type</span></span>

<span data-ttu-id="bc970-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc970-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc970-105">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="bc970-105">The entry point for OneNote resources.</span></span>

<span data-ttu-id="bc970-106">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bc970-106">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="bc970-107">A localização pode ser blocos de anotações do usuário no Microsoft 365 ou no OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="bc970-107">The location can be user notebooks on Microsoft 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Microsoft 365.</span></span> 

<span data-ttu-id="bc970-108">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="bc970-108">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="bc970-109">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bc970-109">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="bc970-110">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bc970-110">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="bc970-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc970-111">Authorization</span></span>

<span data-ttu-id="bc970-112">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="bc970-112">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="bc970-113">Relações</span><span class="sxs-lookup"><span data-stu-id="bc970-113">Relationships</span></span>
| <span data-ttu-id="bc970-114">Relação</span><span class="sxs-lookup"><span data-stu-id="bc970-114">Relationship</span></span> | <span data-ttu-id="bc970-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc970-115">Type</span></span>   |<span data-ttu-id="bc970-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc970-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc970-117">notebooks</span><span class="sxs-lookup"><span data-stu-id="bc970-117">notebooks</span></span>|<span data-ttu-id="bc970-118">Coleção [bloco de anotações](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-118">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="bc970-119">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="bc970-119">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="bc970-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-120">Read-only.</span></span> <span data-ttu-id="bc970-121">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-121">Nullable.</span></span>|
|<span data-ttu-id="bc970-122">operations</span><span class="sxs-lookup"><span data-stu-id="bc970-122">operations</span></span>|<span data-ttu-id="bc970-123">coleção [onenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-123">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="bc970-124">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="bc970-124">The status of OneNote operations.</span></span> <span data-ttu-id="bc970-125">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="bc970-125">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="bc970-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-126">Read-only.</span></span> <span data-ttu-id="bc970-127">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-127">Nullable.</span></span>|
|<span data-ttu-id="bc970-128">páginas</span><span class="sxs-lookup"><span data-stu-id="bc970-128">pages</span></span>|<span data-ttu-id="bc970-129">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-129">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="bc970-130">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="bc970-130">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="bc970-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-131">Read-only.</span></span> <span data-ttu-id="bc970-132">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-132">Nullable.</span></span>|
|<span data-ttu-id="bc970-133">recursos</span><span class="sxs-lookup"><span data-stu-id="bc970-133">resources</span></span>|<span data-ttu-id="bc970-134">coleção [onenoteResource](onenoteresource.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-134">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="bc970-135">A imagem e outros recursos de arquivos nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="bc970-135">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="bc970-136">Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](onenoteresource.md).</span><span class="sxs-lookup"><span data-stu-id="bc970-136">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="bc970-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-137">Read-only.</span></span> <span data-ttu-id="bc970-138">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-138">Nullable.</span></span>|
|<span data-ttu-id="bc970-139">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="bc970-139">sectionGroups</span></span>|<span data-ttu-id="bc970-140">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-140">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="bc970-141">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="bc970-141">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="bc970-142">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-142">Read-only.</span></span> <span data-ttu-id="bc970-143">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-143">Nullable.</span></span>|
|<span data-ttu-id="bc970-144">seções</span><span class="sxs-lookup"><span data-stu-id="bc970-144">sections</span></span>|<span data-ttu-id="bc970-145">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-145">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="bc970-146">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="bc970-146">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="bc970-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bc970-147">Read-only.</span></span> <span data-ttu-id="bc970-148">Anulável.</span><span class="sxs-lookup"><span data-stu-id="bc970-148">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="bc970-149">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc970-149">Methods</span></span>

| <span data-ttu-id="bc970-150">Método</span><span class="sxs-lookup"><span data-stu-id="bc970-150">Method</span></span>           | <span data-ttu-id="bc970-151">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc970-151">Return Type</span></span>    |<span data-ttu-id="bc970-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc970-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bc970-153">Create notebook</span><span class="sxs-lookup"><span data-stu-id="bc970-153">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="bc970-154">bloco de anotações</span><span class="sxs-lookup"><span data-stu-id="bc970-154">notebook</span></span>](notebook.md)| <span data-ttu-id="bc970-155">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="bc970-155">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="bc970-156">List notebooks</span><span class="sxs-lookup"><span data-stu-id="bc970-156">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="bc970-157">Coleção [bloco de anotações](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-157">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="bc970-158">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="bc970-158">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="bc970-159">Create page</span><span class="sxs-lookup"><span data-stu-id="bc970-159">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="bc970-160">onenotePage</span><span class="sxs-lookup"><span data-stu-id="bc970-160">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="bc970-161">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="bc970-161">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="bc970-162">List pages</span><span class="sxs-lookup"><span data-stu-id="bc970-162">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="bc970-163">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-163">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="bc970-164">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="bc970-164">Get a collection of pages.</span></span>|
|[<span data-ttu-id="bc970-165">List section groups</span><span class="sxs-lookup"><span data-stu-id="bc970-165">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="bc970-166">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-166">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="bc970-167">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="bc970-167">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="bc970-168">Listar seções</span><span class="sxs-lookup"><span data-stu-id="bc970-168">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="bc970-169">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="bc970-169">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="bc970-170">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="bc970-170">Get a collection of sections.</span></span>|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
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
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


