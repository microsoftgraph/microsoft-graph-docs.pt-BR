---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 44dfe7b33632bb6691802e46b66f54015b6aa6ae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341488"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="c20cf-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="c20cf-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c20cf-104">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c20cf-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="c20cf-105">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c20cf-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="c20cf-106">A localização pode ser blocos de anotações do usuário no Office 365 ou de consumidor do OneDrive, blocos de anotações de grupo ou blocos de anotações hospedado no site da equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="c20cf-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="c20cf-107">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="c20cf-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="c20cf-108">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c20cf-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="c20cf-109">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="c20cf-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="c20cf-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="c20cf-110">Authorization</span></span>

<span data-ttu-id="c20cf-111">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="c20cf-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="c20cf-112">Relações</span><span class="sxs-lookup"><span data-stu-id="c20cf-112">Relationships</span></span>
| <span data-ttu-id="c20cf-113">Relação</span><span class="sxs-lookup"><span data-stu-id="c20cf-113">Relationship</span></span> | <span data-ttu-id="c20cf-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c20cf-114">Type</span></span>   |<span data-ttu-id="c20cf-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c20cf-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c20cf-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="c20cf-116">notebooks</span></span>|<span data-ttu-id="c20cf-117">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-117">[notebook](notebook.md) collection</span></span>|<span data-ttu-id="c20cf-118">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c20cf-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="c20cf-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-119">Read-only.</span></span> <span data-ttu-id="c20cf-120">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-120">Nullable.</span></span>|
|<span data-ttu-id="c20cf-121">operations</span><span class="sxs-lookup"><span data-stu-id="c20cf-121">operations</span></span>|<span data-ttu-id="c20cf-122">coleção [onenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-122">[onenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="c20cf-123">O status das operações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c20cf-123">The status of OneNote operations.</span></span> <span data-ttu-id="c20cf-124">Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="c20cf-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="c20cf-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-125">Read-only.</span></span> <span data-ttu-id="c20cf-126">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-126">Nullable.</span></span>|
|<span data-ttu-id="c20cf-127">páginas</span><span class="sxs-lookup"><span data-stu-id="c20cf-127">pages</span></span>|<span data-ttu-id="c20cf-128">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-128">[onenotePage](onenotepage.md) collection</span></span>|<span data-ttu-id="c20cf-129">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c20cf-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c20cf-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-130">Read-only.</span></span> <span data-ttu-id="c20cf-131">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-131">Nullable.</span></span>|
|<span data-ttu-id="c20cf-132">recursos</span><span class="sxs-lookup"><span data-stu-id="c20cf-132">resources</span></span>|<span data-ttu-id="c20cf-133">coleção [onenoteResource](onenoteresource.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-133">[onenoteResource](onenoteresource.md) collection</span></span> |<span data-ttu-id="c20cf-134">A imagem e outros recursos de arquivos nas páginas do OneNote.</span><span class="sxs-lookup"><span data-stu-id="c20cf-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="c20cf-135">Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](onenoteresource.md).</span><span class="sxs-lookup"><span data-stu-id="c20cf-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](onenoteresource.md).</span></span> <span data-ttu-id="c20cf-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-136">Read-only.</span></span> <span data-ttu-id="c20cf-137">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-137">Nullable.</span></span>|
|<span data-ttu-id="c20cf-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="c20cf-138">sectionGroups</span></span>|<span data-ttu-id="c20cf-139">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-139">[sectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="c20cf-140">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c20cf-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c20cf-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-141">Read-only.</span></span> <span data-ttu-id="c20cf-142">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-142">Nullable.</span></span>|
|<span data-ttu-id="c20cf-143">seções</span><span class="sxs-lookup"><span data-stu-id="c20cf-143">sections</span></span>|<span data-ttu-id="c20cf-144">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-144">[onenoteSection](onenotesection.md) collection</span></span>|<span data-ttu-id="c20cf-145">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.</span><span class="sxs-lookup"><span data-stu-id="c20cf-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="c20cf-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c20cf-146">Read-only.</span></span> <span data-ttu-id="c20cf-147">Anulável.</span><span class="sxs-lookup"><span data-stu-id="c20cf-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="c20cf-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="c20cf-148">Methods</span></span>

| <span data-ttu-id="c20cf-149">Método</span><span class="sxs-lookup"><span data-stu-id="c20cf-149">Method</span></span>           | <span data-ttu-id="c20cf-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c20cf-150">Return Type</span></span>    |<span data-ttu-id="c20cf-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="c20cf-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c20cf-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="c20cf-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="c20cf-153">anotações</span><span class="sxs-lookup"><span data-stu-id="c20cf-153">notebook</span></span>](notebook.md)| <span data-ttu-id="c20cf-154">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="c20cf-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="c20cf-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="c20cf-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="c20cf-156">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-156">[notebook](notebook.md) collection</span></span>| <span data-ttu-id="c20cf-157">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="c20cf-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="c20cf-158">Create page</span><span class="sxs-lookup"><span data-stu-id="c20cf-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="c20cf-159">onenotePage</span><span class="sxs-lookup"><span data-stu-id="c20cf-159">onenotePage</span></span>](onenotepage.md) | <span data-ttu-id="c20cf-160">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="c20cf-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="c20cf-161">List pages</span><span class="sxs-lookup"><span data-stu-id="c20cf-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="c20cf-162">coleção [onenotePage](onenotepage.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-162">[onenotePage](onenotepage.md)  collection</span></span>| <span data-ttu-id="c20cf-163">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="c20cf-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="c20cf-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="c20cf-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="c20cf-165">coleção de [seções](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-165">[sectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="c20cf-166">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="c20cf-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="c20cf-167">Listar seções</span><span class="sxs-lookup"><span data-stu-id="c20cf-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="c20cf-168">coleção [onenoteSection](onenotesection.md)</span><span class="sxs-lookup"><span data-stu-id="c20cf-168">[onenoteSection](onenotesection.md) collection</span></span>| <span data-ttu-id="c20cf-169">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="c20cf-169">Get a collection of sections.</span></span>|
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
