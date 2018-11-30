---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
ms.openlocfilehash: c1b875b686015df8134103b0793a1e342e7f4b89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035323"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="bd2d0-103">tipo de recurso do onenote</span><span class="sxs-lookup"><span data-stu-id="bd2d0-103">onenote resource type</span></span>

> <span data-ttu-id="bd2d0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd2d0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd2d0-106">O ponto de entrada para os recursos do OneNote.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="bd2d0-107">Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bd2d0-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="bd2d0-108">O local pode ser blocos de anotações do usuário no Office 365 ou consumidor OneDrive, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="bd2d0-109">**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:</span><span class="sxs-lookup"><span data-stu-id="bd2d0-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="bd2d0-110">**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bd2d0-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="bd2d0-111">**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:</span><span class="sxs-lookup"><span data-stu-id="bd2d0-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="bd2d0-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd2d0-112">Authorization</span></span>

<span data-ttu-id="bd2d0-113">Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="bd2d0-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="bd2d0-114">Relações</span><span class="sxs-lookup"><span data-stu-id="bd2d0-114">Relationships</span></span>
| <span data-ttu-id="bd2d0-115">Relação</span><span class="sxs-lookup"><span data-stu-id="bd2d0-115">Relationship</span></span> | <span data-ttu-id="bd2d0-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd2d0-116">Type</span></span>   |<span data-ttu-id="bd2d0-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd2d0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd2d0-118">notebooks</span><span class="sxs-lookup"><span data-stu-id="bd2d0-118">notebooks</span></span>|<span data-ttu-id="bd2d0-119">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="bd2d0-p102">A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd2d0-123">operations</span><span class="sxs-lookup"><span data-stu-id="bd2d0-123">operations</span></span>|<span data-ttu-id="bd2d0-124">Coleção [Operation](onenoteoperation.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="bd2d0-p103">O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd2d0-129">páginas</span><span class="sxs-lookup"><span data-stu-id="bd2d0-129">pages</span></span>|<span data-ttu-id="bd2d0-130">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-130">[Page](page.md) collection</span></span>|<span data-ttu-id="bd2d0-p104">As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd2d0-134">recursos</span><span class="sxs-lookup"><span data-stu-id="bd2d0-134">resources</span></span>|<span data-ttu-id="bd2d0-135">Coleção [Resource](resource.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="bd2d0-p105">A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd2d0-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="bd2d0-140">sectionGroups</span></span>|<span data-ttu-id="bd2d0-141">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="bd2d0-p106">Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="bd2d0-145">sections</span><span class="sxs-lookup"><span data-stu-id="bd2d0-145">sections</span></span>|<span data-ttu-id="bd2d0-146">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-146">[Section](section.md) collection</span></span>|<span data-ttu-id="bd2d0-p107">As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="bd2d0-150">Métodos</span><span class="sxs-lookup"><span data-stu-id="bd2d0-150">Methods</span></span>

| <span data-ttu-id="bd2d0-151">Método</span><span class="sxs-lookup"><span data-stu-id="bd2d0-151">Method</span></span>           | <span data-ttu-id="bd2d0-152">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bd2d0-152">Return Type</span></span>    |<span data-ttu-id="bd2d0-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd2d0-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bd2d0-154">Create notebook</span><span class="sxs-lookup"><span data-stu-id="bd2d0-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="bd2d0-155">Notebook</span><span class="sxs-lookup"><span data-stu-id="bd2d0-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="bd2d0-156">Crie um bloco de anotações postando na coleção notebooks.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="bd2d0-157">List notebooks</span><span class="sxs-lookup"><span data-stu-id="bd2d0-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="bd2d0-158">Coleção [Notebook](notebook.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="bd2d0-159">Obter uma coleção de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="bd2d0-160">Create page</span><span class="sxs-lookup"><span data-stu-id="bd2d0-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="bd2d0-161">Page</span><span class="sxs-lookup"><span data-stu-id="bd2d0-161">Page</span></span>](page.md)| <span data-ttu-id="bd2d0-162">Crie uma página postando na coleção pages.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="bd2d0-163">List pages</span><span class="sxs-lookup"><span data-stu-id="bd2d0-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="bd2d0-164">Coleção [Page](page.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-164">[Page](page.md) collection</span></span>| <span data-ttu-id="bd2d0-165">Obter uma coleção de páginas.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="bd2d0-166">List section groups</span><span class="sxs-lookup"><span data-stu-id="bd2d0-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="bd2d0-167">Coleção [SectionGroup](sectiongroup.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="bd2d0-168">Obter uma coleção de grupos de seção.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="bd2d0-169">List sections</span><span class="sxs-lookup"><span data-stu-id="bd2d0-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="bd2d0-170">Coleção [Section](section.md)</span><span class="sxs-lookup"><span data-stu-id="bd2d0-170">[Section](section.md) collection</span></span>| <span data-ttu-id="bd2d0-171">Obter uma coleção de seções.</span><span class="sxs-lookup"><span data-stu-id="bd2d0-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
