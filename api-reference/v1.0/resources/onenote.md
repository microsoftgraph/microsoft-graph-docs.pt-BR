---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: Jewan-microsoft
ms.openlocfilehash: 9570b99aad96196af6d21f41352dada9f4b869b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343649"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="e4d7d-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="e4d7d-103">onenote resource type</span></span>

<span data-ttu-id="e4d7d-104">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="e4d7d-105">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="e4d7d-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="e4d7d-106">A localização pode ser blocos de anotações do usuário no Office 365 ou OneDrive do consumidor, blocos de anotações de grupo ou blocos de anotações hospedado no site de equipe do SharePoint no Office 365.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="e4d7d-107">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="e4d7d-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="e4d7d-108">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="e4d7d-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="e4d7d-109">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="e4d7d-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="e4d7d-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4d7d-110">Authorization</span></span>

<span data-ttu-id="e4d7d-111">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="e4d7d-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="e4d7d-112">Relações</span><span class="sxs-lookup"><span data-stu-id="e4d7d-112">Relationships</span></span>
| <span data-ttu-id="e4d7d-113">Relação</span><span class="sxs-lookup"><span data-stu-id="e4d7d-113">Relationship</span></span> | <span data-ttu-id="e4d7d-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4d7d-114">Type</span></span>   |<span data-ttu-id="e4d7d-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d7d-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4d7d-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="e4d7d-116">notebooks</span></span>|<span data-ttu-id="e4d7d-117">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="e4d7d-p101">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4d7d-121">operations</span><span class="sxs-lookup"><span data-stu-id="e4d7d-121">operations</span></span>|<span data-ttu-id="e4d7d-122">Coleção [OnenoteOperation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="e4d7d-p102">O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4d7d-127">páginas</span><span class="sxs-lookup"><span data-stu-id="e4d7d-127">pages</span></span>|<span data-ttu-id="e4d7d-128">Coleção [OnenotePage](page.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="e4d7d-p103">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4d7d-132">recursos</span><span class="sxs-lookup"><span data-stu-id="e4d7d-132">resources</span></span>|<span data-ttu-id="e4d7d-133">Coleção [OnenoteResource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="e4d7d-p104">A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4d7d-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e4d7d-138">sectionGroups</span></span>|<span data-ttu-id="e4d7d-139">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e4d7d-p105">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e4d7d-143">sections</span><span class="sxs-lookup"><span data-stu-id="e4d7d-143">sections</span></span>|<span data-ttu-id="e4d7d-144">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="e4d7d-p106">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e4d7d-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="e4d7d-148">Methods</span></span>

| <span data-ttu-id="e4d7d-149">Método</span><span class="sxs-lookup"><span data-stu-id="e4d7d-149">Method</span></span>           | <span data-ttu-id="e4d7d-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e4d7d-150">Return Type</span></span>    |<span data-ttu-id="e4d7d-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4d7d-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4d7d-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="e4d7d-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="e4d7d-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="e4d7d-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="e4d7d-154">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="e4d7d-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="e4d7d-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="e4d7d-156">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="e4d7d-157">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="e4d7d-158">Create page</span><span class="sxs-lookup"><span data-stu-id="e4d7d-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="e4d7d-159">Page</span><span class="sxs-lookup"><span data-stu-id="e4d7d-159">Page</span></span>](page.md)| <span data-ttu-id="e4d7d-160">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="e4d7d-161">List pages</span><span class="sxs-lookup"><span data-stu-id="e4d7d-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="e4d7d-162">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-162">[Page](page.md) collection</span></span>| <span data-ttu-id="e4d7d-163">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="e4d7d-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="e4d7d-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="e4d7d-165">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e4d7d-166">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="e4d7d-167">List sections</span><span class="sxs-lookup"><span data-stu-id="e4d7d-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="e4d7d-168">Coleção [OnenoteSection](section.md)</span><span class="sxs-lookup"><span data-stu-id="e4d7d-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="e4d7d-169">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e4d7d-170">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4d7d-170">JSON Representation</span></span>
<span data-ttu-id="e4d7d-171">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4d7d-171">Here is a JSON representation of the resource.</span></span>
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
