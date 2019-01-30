---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640095"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="16219-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="16219-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16219-104">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="16219-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="16219-105">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="16219-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="16219-106">O local pode ser blocos de anotações do usuário no Office 365 ou consumidor OneDrive, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365.</span><span class="sxs-lookup"><span data-stu-id="16219-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="16219-107">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="16219-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="16219-108">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="16219-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="16219-109">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="16219-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="16219-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="16219-110">Authorization</span></span>

<span data-ttu-id="16219-111">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="16219-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="16219-112">Relações</span><span class="sxs-lookup"><span data-stu-id="16219-112">Relationships</span></span>
| <span data-ttu-id="16219-113">Relação</span><span class="sxs-lookup"><span data-stu-id="16219-113">Relationship</span></span> | <span data-ttu-id="16219-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="16219-114">Type</span></span>   |<span data-ttu-id="16219-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="16219-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16219-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="16219-116">notebooks</span></span>|<span data-ttu-id="16219-117">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="16219-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="16219-p101">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="16219-121">operations</span><span class="sxs-lookup"><span data-stu-id="16219-121">operations</span></span>|<span data-ttu-id="16219-122">Coleção [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="16219-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="16219-p102">O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="16219-127">páginas</span><span class="sxs-lookup"><span data-stu-id="16219-127">pages</span></span>|<span data-ttu-id="16219-128">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="16219-128">[Page](page.md) collection</span></span>|<span data-ttu-id="16219-p103">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="16219-132">recursos</span><span class="sxs-lookup"><span data-stu-id="16219-132">resources</span></span>|<span data-ttu-id="16219-133">Coleção [Resource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="16219-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="16219-p104">A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="16219-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="16219-138">sectionGroups</span></span>|<span data-ttu-id="16219-139">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="16219-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="16219-p105">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="16219-143">sections</span><span class="sxs-lookup"><span data-stu-id="16219-143">sections</span></span>|<span data-ttu-id="16219-144">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="16219-144">[Section](section.md) collection</span></span>|<span data-ttu-id="16219-p106">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="16219-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="16219-148">Métodos</span><span class="sxs-lookup"><span data-stu-id="16219-148">Methods</span></span>

| <span data-ttu-id="16219-149">Método</span><span class="sxs-lookup"><span data-stu-id="16219-149">Method</span></span>           | <span data-ttu-id="16219-150">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16219-150">Return Type</span></span>    |<span data-ttu-id="16219-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="16219-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16219-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="16219-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="16219-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="16219-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="16219-154">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="16219-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="16219-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="16219-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="16219-156">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="16219-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="16219-157">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="16219-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="16219-158">Create page</span><span class="sxs-lookup"><span data-stu-id="16219-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="16219-159">Page</span><span class="sxs-lookup"><span data-stu-id="16219-159">Page</span></span>](page.md)| <span data-ttu-id="16219-160">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="16219-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="16219-161">List pages</span><span class="sxs-lookup"><span data-stu-id="16219-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="16219-162">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="16219-162">[Page](page.md) collection</span></span>| <span data-ttu-id="16219-163">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="16219-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="16219-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="16219-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="16219-165">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="16219-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="16219-166">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="16219-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="16219-167">List sections</span><span class="sxs-lookup"><span data-stu-id="16219-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="16219-168">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="16219-168">[Section](section.md) collection</span></span>| <span data-ttu-id="16219-169">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="16219-169">Get a collection of sections.</span></span>|

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
