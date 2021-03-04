---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 587014aa0c9dbe4c05c0e3b946c3f6e44b7cb821
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442784"
---
# <a name="site-resource-type"></a><span data-ttu-id="e07b1-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="e07b1-103">site resource type</span></span>

<span data-ttu-id="e07b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e07b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e07b1-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e07b1-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="e07b1-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="e07b1-106">Methods</span></span>

| <span data-ttu-id="e07b1-107">Método</span><span class="sxs-lookup"><span data-stu-id="e07b1-107">Method</span></span>                         | <span data-ttu-id="e07b1-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="e07b1-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="e07b1-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-109">[Get root site][]</span></span>              | <span data-ttu-id="e07b1-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="e07b1-110">GET /sites/root</span></span>
| <span data-ttu-id="e07b1-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-111">[Get site][]</span></span>                   | <span data-ttu-id="e07b1-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="e07b1-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="e07b1-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-113">[Get site by path][]</span></span>           | <span data-ttu-id="e07b1-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="e07b1-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="e07b1-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-115">[Get site for a group][]</span></span>       | <span data-ttu-id="e07b1-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="e07b1-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="e07b1-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-117">[Get analytics][]</span></span>              | <span data-ttu-id="e07b1-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="e07b1-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="e07b1-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-119">[Get activities by interval][]</span></span> | <span data-ttu-id="e07b1-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="e07b1-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="e07b1-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-121">[List pages][]</span></span>                 | <span data-ttu-id="e07b1-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="e07b1-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="e07b1-123">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-123">[List root sites][]</span></span>            | <span data-ttu-id="e07b1-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="e07b1-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="e07b1-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-125">[Search for sites][]</span></span>           | <span data-ttu-id="e07b1-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="e07b1-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="e07b1-127">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-127">[Follow site][]</span></span>                | <span data-ttu-id="e07b1-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="e07b1-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="e07b1-129">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-129">[Unfollow site][]</span></span>              | <span data-ttu-id="e07b1-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="e07b1-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="e07b1-131">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-131">[List followed sites][]</span></span>        | <span data-ttu-id="e07b1-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="e07b1-132">GET /me/followedSites</span></span>
| <span data-ttu-id="e07b1-133">[Obter permissão][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-133">[Get permission][]</span></span>             | <span data-ttu-id="e07b1-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="e07b1-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="e07b1-135">[Listar permissões][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-135">[List permissions][]</span></span>           | <span data-ttu-id="e07b1-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="e07b1-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="e07b1-137">[Criar permissões][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-137">[Create permissions][]</span></span>         | <span data-ttu-id="e07b1-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="e07b1-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="e07b1-139">[Excluir permissão][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-139">[Delete permission][]</span></span>         | <span data-ttu-id="e07b1-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="e07b1-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="e07b1-141">[Atualizar permissão][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-141">[Update permission][]</span></span>         | <span data-ttu-id="e07b1-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="e07b1-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

[Obter site]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Lista sites raiz]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Procurar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[Seguir site]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[Deixar de seguir site]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[Listar sites seguidos]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md
[Obter permissão]: ../api/site-get-permission.md
[Get permission]: ../api/site-get-permission.md
[Listar permissões]: ../api/site-list-permissions.md
[List permissions]: ../api/site-list-permissions.md
[Criar permissões]: ../api/site-post-permissions.md
[Create permissions]: ../api/site-post-permissions.md
[Excluir permissão]: ../api/site-delete-permission.md
[Delete permission]: ../api/site-delete-permission.md
[Atualizar permissão]: ../api/site-update-permission.md
[Update permission]: ../api/site-update-permission.md


## <a name="properties"></a><span data-ttu-id="e07b1-160">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e07b1-160">Properties</span></span>

| <span data-ttu-id="e07b1-161">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e07b1-161">Property name</span></span>            | <span data-ttu-id="e07b1-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="e07b1-162">Type</span></span>               | <span data-ttu-id="e07b1-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07b1-163">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="e07b1-164">**id**</span><span class="sxs-lookup"><span data-stu-id="e07b1-164">**id**</span></span>                   | <span data-ttu-id="e07b1-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07b1-165">string</span></span>             | <span data-ttu-id="e07b1-166">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="e07b1-166">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="e07b1-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-167">Read-only.</span></span>
| <span data-ttu-id="e07b1-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e07b1-168">**createdDateTime**</span></span>      | <span data-ttu-id="e07b1-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07b1-169">DateTimeOffset</span></span>     | <span data-ttu-id="e07b1-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e07b1-172">**description**</span><span class="sxs-lookup"><span data-stu-id="e07b1-172">**description**</span></span>          | <span data-ttu-id="e07b1-173">string</span><span class="sxs-lookup"><span data-stu-id="e07b1-173">string</span></span>             | <span data-ttu-id="e07b1-174">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-174">The descriptive text for the site.</span></span>
| <span data-ttu-id="e07b1-175">**eTag**</span><span class="sxs-lookup"><span data-stu-id="e07b1-175">**eTag**</span></span>                 | <span data-ttu-id="e07b1-176">string</span><span class="sxs-lookup"><span data-stu-id="e07b1-176">string</span></span>             | <span data-ttu-id="e07b1-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="e07b1-179">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e07b1-179">**displayName**</span></span>          | <span data-ttu-id="e07b1-180">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e07b1-180">string</span></span>             | <span data-ttu-id="e07b1-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="e07b1-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e07b1-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e07b1-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07b1-184">DateTimeOffset</span></span>     | <span data-ttu-id="e07b1-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e07b1-187">**name**</span><span class="sxs-lookup"><span data-stu-id="e07b1-187">**name**</span></span>                 | <span data-ttu-id="e07b1-188">string</span><span class="sxs-lookup"><span data-stu-id="e07b1-188">string</span></span>             | <span data-ttu-id="e07b1-189">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="e07b1-189">The name / title of the item.</span></span>
| <span data-ttu-id="e07b1-190">**root**</span><span class="sxs-lookup"><span data-stu-id="e07b1-190">**root**</span></span>                 | <span data-ttu-id="e07b1-191">[root][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-191">[root][]</span></span>           | <span data-ttu-id="e07b1-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="e07b1-194">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="e07b1-194">**sharepointIds**</span></span>        | <span data-ttu-id="e07b1-195">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-195">[sharepointIds][]</span></span>  | <span data-ttu-id="e07b1-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e07b1-198">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="e07b1-198">**siteCollection**</span></span>       | <span data-ttu-id="e07b1-199">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-199">[siteCollection][]</span></span> | <span data-ttu-id="e07b1-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="e07b1-203">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e07b1-203">**webUrl**</span></span>               | <span data-ttu-id="e07b1-204">string (url)</span><span class="sxs-lookup"><span data-stu-id="e07b1-204">string (url)</span></span>       | <span data-ttu-id="e07b1-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="e07b1-207">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="e07b1-207">id property</span></span>
<span data-ttu-id="e07b1-208">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="e07b1-208">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="e07b1-209">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="e07b1-209">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e07b1-210">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="e07b1-210">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="e07b1-211">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="e07b1-211">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="e07b1-212">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="e07b1-212">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e07b1-213">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="e07b1-213">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e07b1-214">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="e07b1-214">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="e07b1-215">Relações</span><span class="sxs-lookup"><span data-stu-id="e07b1-215">Relationships</span></span>

| <span data-ttu-id="e07b1-216">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="e07b1-216">Relationship name</span></span> | <span data-ttu-id="e07b1-217">Tipo</span><span class="sxs-lookup"><span data-stu-id="e07b1-217">Type</span></span>                             | <span data-ttu-id="e07b1-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="e07b1-218">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="e07b1-219">**analytics**</span><span class="sxs-lookup"><span data-stu-id="e07b1-219">**analytics**</span></span>     | <span data-ttu-id="e07b1-220">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="e07b1-220">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="e07b1-221">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-221">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="e07b1-222">**columns**</span><span class="sxs-lookup"><span data-stu-id="e07b1-222">**columns**</span></span>       | <span data-ttu-id="e07b1-223">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-223">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e07b1-224">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-224">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="e07b1-225">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e07b1-225">**contentTypes**</span></span>  | <span data-ttu-id="e07b1-226">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-226">Collection([contentType][])</span></span>      | <span data-ttu-id="e07b1-227">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-227">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="e07b1-228">**drive**</span><span class="sxs-lookup"><span data-stu-id="e07b1-228">**drive**</span></span>         | <span data-ttu-id="e07b1-229">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e07b1-229">[drive][]</span></span>                        | <span data-ttu-id="e07b1-230">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-230">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="e07b1-231">**drives**</span><span class="sxs-lookup"><span data-stu-id="e07b1-231">**drives**</span></span>        | <span data-ttu-id="e07b1-232">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-232">Collection([drive][])</span></span>            | <span data-ttu-id="e07b1-233">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-233">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="e07b1-234">**items**</span><span class="sxs-lookup"><span data-stu-id="e07b1-234">**items**</span></span>         | <span data-ttu-id="e07b1-235">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-235">Collection([baseItem][])</span></span>         | <span data-ttu-id="e07b1-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="e07b1-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e07b1-238">**lists**</span><span class="sxs-lookup"><span data-stu-id="e07b1-238">**lists**</span></span>         | <span data-ttu-id="e07b1-239">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-239">Collection([list][])</span></span>             | <span data-ttu-id="e07b1-240">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-240">The collection of lists under this site.</span></span>
| <span data-ttu-id="e07b1-241">**pages**</span><span class="sxs-lookup"><span data-stu-id="e07b1-241">**pages**</span></span>         | <span data-ttu-id="e07b1-242">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-242">Collection([sitePage][])</span></span>         | <span data-ttu-id="e07b1-243">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-243">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="e07b1-244">**permissões**</span><span class="sxs-lookup"><span data-stu-id="e07b1-244">**permissions**</span></span>   | <span data-ttu-id="e07b1-245">Coleção ([permissão][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-245">Collection([permission][])</span></span>         | <span data-ttu-id="e07b1-246">As permissões associadas ao site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-246">The permissions associated with the site.</span></span> <span data-ttu-id="e07b1-247">Anulável.</span><span class="sxs-lookup"><span data-stu-id="e07b1-247">Nullable.</span></span>
| <span data-ttu-id="e07b1-248">**sites**</span><span class="sxs-lookup"><span data-stu-id="e07b1-248">**sites**</span></span>         | <span data-ttu-id="e07b1-249">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-249">Collection([site][])</span></span>             | <span data-ttu-id="e07b1-250">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="e07b1-250">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="e07b1-251">**externalColumns**</span><span class="sxs-lookup"><span data-stu-id="e07b1-251">**externalColumns**</span></span>     | <span data-ttu-id="e07b1-252">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e07b1-252">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="e07b1-253">A coleção de definições de coluna disponíveis no site que são referenciadas nos sites na hierarquia pai do site atual.</span><span class="sxs-lookup"><span data-stu-id="e07b1-253">The collection of column definitions available in the site that are referenced from the sites in the parent hierarchy of the current site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permissão]: permission.md
[permission]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="e07b1-266">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e07b1-266">JSON representation</span></span>

<span data-ttu-id="e07b1-267">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="e07b1-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="e07b1-268">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="e07b1-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "permissions",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
