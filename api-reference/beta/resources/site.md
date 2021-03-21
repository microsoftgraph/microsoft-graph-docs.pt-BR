---
author: JeremyKelley
description: O recurso site fornece metadados e relações para um site do SharePoint.
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: e754bf9e5199de502672cdf0a0de5279eb5ef80f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953744"
---
# <a name="site-resource-type"></a><span data-ttu-id="78230-103">tipo de recurso do site</span><span class="sxs-lookup"><span data-stu-id="78230-103">site resource type</span></span>

<span data-ttu-id="78230-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78230-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78230-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="78230-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="78230-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="78230-106">Methods</span></span>

| <span data-ttu-id="78230-107">Método</span><span class="sxs-lookup"><span data-stu-id="78230-107">Method</span></span>                         | <span data-ttu-id="78230-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="78230-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="78230-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="78230-109">[Get root site][]</span></span>              | <span data-ttu-id="78230-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="78230-110">GET /sites/root</span></span>
| <span data-ttu-id="78230-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="78230-111">[Get site][]</span></span>                   | <span data-ttu-id="78230-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="78230-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="78230-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="78230-113">[Get site by path][]</span></span>           | <span data-ttu-id="78230-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="78230-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="78230-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="78230-115">[Get site for a group][]</span></span>       | <span data-ttu-id="78230-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="78230-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="78230-117">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="78230-117">[Get analytics][]</span></span>              | <span data-ttu-id="78230-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="78230-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="78230-119">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="78230-119">[Get activities by interval][]</span></span> | <span data-ttu-id="78230-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="78230-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="78230-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="78230-121">[List pages][]</span></span>                 | <span data-ttu-id="78230-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="78230-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="78230-123">[Lista sites raiz][]</span><span class="sxs-lookup"><span data-stu-id="78230-123">[List root sites][]</span></span>            | <span data-ttu-id="78230-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="78230-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="78230-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="78230-125">[Search for sites][]</span></span>           | <span data-ttu-id="78230-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="78230-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="78230-127">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="78230-127">[Follow site][]</span></span>                | <span data-ttu-id="78230-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="78230-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="78230-129">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="78230-129">[Unfollow site][]</span></span>              | <span data-ttu-id="78230-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="78230-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="78230-131">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="78230-131">[List followed sites][]</span></span>        | <span data-ttu-id="78230-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="78230-132">GET /me/followedSites</span></span>
| <span data-ttu-id="78230-133">[Obter permissão][]</span><span class="sxs-lookup"><span data-stu-id="78230-133">[Get permission][]</span></span>             | <span data-ttu-id="78230-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="78230-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="78230-135">[Listar permissões][]</span><span class="sxs-lookup"><span data-stu-id="78230-135">[List permissions][]</span></span>           | <span data-ttu-id="78230-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="78230-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="78230-137">[Criar permissões][]</span><span class="sxs-lookup"><span data-stu-id="78230-137">[Create permissions][]</span></span>         | <span data-ttu-id="78230-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="78230-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="78230-139">[Excluir permissão][]</span><span class="sxs-lookup"><span data-stu-id="78230-139">[Delete permission][]</span></span>         | <span data-ttu-id="78230-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="78230-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="78230-141">[Atualizar permissão][]</span><span class="sxs-lookup"><span data-stu-id="78230-141">[Update permission][]</span></span>         | <span data-ttu-id="78230-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="78230-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>
|<span data-ttu-id="78230-143">[Tipos de conteúdo de lista][]</span><span class="sxs-lookup"><span data-stu-id="78230-143">[List content types][]</span></span>          | <span data-ttu-id="78230-144">Obter /sites/{site-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="78230-144">GET /sites/{site-id}/contentTypes</span></span>
|<span data-ttu-id="78230-145">[Criar contentType][]</span><span class="sxs-lookup"><span data-stu-id="78230-145">[Create contentType][]</span></span>        | <span data-ttu-id="78230-146">POSTAR /sites/{site-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="78230-146">POST /sites/{site-id}/contentTypes</span></span>
|<span data-ttu-id="78230-147">[Colunas de lista][]</span><span class="sxs-lookup"><span data-stu-id="78230-147">[List columns][]</span></span>               | <span data-ttu-id="78230-148">OBTER /sites/{site-id}/columns</span><span class="sxs-lookup"><span data-stu-id="78230-148">GET /sites/{site-id}/columns</span></span>
|<span data-ttu-id="78230-149">[Criar coluna][]</span><span class="sxs-lookup"><span data-stu-id="78230-149">[Create column][]</span></span>              | <span data-ttu-id="78230-150">POSTAR /sites/{site-id}/columns</span><span class="sxs-lookup"><span data-stu-id="78230-150">POST /sites/{site-id}/columns</span></span>

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
[Tipos de conteúdo de lista]: ../api/site-list-contenttypes.md
[List content types]: ../api/site-list-contenttypes.md
[Criar contentType]: ../api/site-post-contenttypes.md
[Create contentType]: ../api/site-post-contenttypes.md
[Colunas de lista]: ../api/site-list-columns.md
[List columns]: ../api/site-list-columns.md
[Criar coluna]: ../api/site-post-columns.md
[Create column]: ../api/site-post-columns.md


## <a name="properties"></a><span data-ttu-id="78230-172">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78230-172">Properties</span></span>

| <span data-ttu-id="78230-173">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="78230-173">Property name</span></span>            | <span data-ttu-id="78230-174">Tipo</span><span class="sxs-lookup"><span data-stu-id="78230-174">Type</span></span>               | <span data-ttu-id="78230-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="78230-175">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="78230-176">**id**</span><span class="sxs-lookup"><span data-stu-id="78230-176">**id**</span></span>                   | <span data-ttu-id="78230-177">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78230-177">string</span></span>             | <span data-ttu-id="78230-178">O [identificador exclusivo](#id-property) do item.</span><span class="sxs-lookup"><span data-stu-id="78230-178">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="78230-179">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-179">Read-only.</span></span>
| <span data-ttu-id="78230-180">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="78230-180">**createdDateTime**</span></span>      | <span data-ttu-id="78230-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78230-181">DateTimeOffset</span></span>     | <span data-ttu-id="78230-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="78230-184">**description**</span><span class="sxs-lookup"><span data-stu-id="78230-184">**description**</span></span>          | <span data-ttu-id="78230-185">string</span><span class="sxs-lookup"><span data-stu-id="78230-185">string</span></span>             | <span data-ttu-id="78230-186">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="78230-186">The descriptive text for the site.</span></span>
| <span data-ttu-id="78230-187">**eTag**</span><span class="sxs-lookup"><span data-stu-id="78230-187">**eTag**</span></span>                 | <span data-ttu-id="78230-188">string</span><span class="sxs-lookup"><span data-stu-id="78230-188">string</span></span>             | <span data-ttu-id="78230-p103">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="78230-191">**displayName**</span><span class="sxs-lookup"><span data-stu-id="78230-191">**displayName**</span></span>          | <span data-ttu-id="78230-192">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78230-192">string</span></span>             | <span data-ttu-id="78230-p104">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="78230-195">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="78230-195">**lastModifiedDateTime**</span></span> | <span data-ttu-id="78230-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78230-196">DateTimeOffset</span></span>     | <span data-ttu-id="78230-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="78230-199">**name**</span><span class="sxs-lookup"><span data-stu-id="78230-199">**name**</span></span>                 | <span data-ttu-id="78230-200">string</span><span class="sxs-lookup"><span data-stu-id="78230-200">string</span></span>             | <span data-ttu-id="78230-201">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="78230-201">The name / title of the item.</span></span>
| <span data-ttu-id="78230-202">**root**</span><span class="sxs-lookup"><span data-stu-id="78230-202">**root**</span></span>                 | <span data-ttu-id="78230-203">[root][]</span><span class="sxs-lookup"><span data-stu-id="78230-203">[root][]</span></span>           | <span data-ttu-id="78230-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="78230-206">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="78230-206">**sharepointIds**</span></span>        | <span data-ttu-id="78230-207">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="78230-207">[sharepointIds][]</span></span>  | <span data-ttu-id="78230-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="78230-210">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="78230-210">**siteCollection**</span></span>       | <span data-ttu-id="78230-211">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="78230-211">[siteCollection][]</span></span> | <span data-ttu-id="78230-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="78230-215">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="78230-215">**webUrl**</span></span>               | <span data-ttu-id="78230-216">string (url)</span><span class="sxs-lookup"><span data-stu-id="78230-216">string (url)</span></span>       | <span data-ttu-id="78230-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="78230-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="78230-219">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="78230-219">id property</span></span>
<span data-ttu-id="78230-220">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="78230-220">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="78230-221">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="78230-221">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="78230-222">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="78230-222">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="78230-223">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="78230-223">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="78230-224">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="78230-224">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="78230-225">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="78230-225">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="78230-226">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="78230-226">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="78230-227">Relações</span><span class="sxs-lookup"><span data-stu-id="78230-227">Relationships</span></span>

| <span data-ttu-id="78230-228">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="78230-228">Relationship name</span></span> | <span data-ttu-id="78230-229">Tipo</span><span class="sxs-lookup"><span data-stu-id="78230-229">Type</span></span>                             | <span data-ttu-id="78230-230">Descrição</span><span class="sxs-lookup"><span data-stu-id="78230-230">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="78230-231">**analytics**</span><span class="sxs-lookup"><span data-stu-id="78230-231">**analytics**</span></span>     | <span data-ttu-id="78230-232">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="78230-232">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="78230-233">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="78230-233">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="78230-234">**columns**</span><span class="sxs-lookup"><span data-stu-id="78230-234">**columns**</span></span>       | <span data-ttu-id="78230-235">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="78230-235">Collection([columnDefinition][])</span></span> | <span data-ttu-id="78230-236">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="78230-236">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="78230-237">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="78230-237">**contentTypes**</span></span>  | <span data-ttu-id="78230-238">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="78230-238">Collection([contentType][])</span></span>      | <span data-ttu-id="78230-239">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="78230-239">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="78230-240">**drive**</span><span class="sxs-lookup"><span data-stu-id="78230-240">**drive**</span></span>         | <span data-ttu-id="78230-241">[drive][]</span><span class="sxs-lookup"><span data-stu-id="78230-241">[drive][]</span></span>                        | <span data-ttu-id="78230-242">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="78230-242">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="78230-243">**drives**</span><span class="sxs-lookup"><span data-stu-id="78230-243">**drives**</span></span>        | <span data-ttu-id="78230-244">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="78230-244">Collection([drive][])</span></span>            | <span data-ttu-id="78230-245">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="78230-245">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="78230-246">**items**</span><span class="sxs-lookup"><span data-stu-id="78230-246">**items**</span></span>         | <span data-ttu-id="78230-247">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="78230-247">Collection([baseItem][])</span></span>         | <span data-ttu-id="78230-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="78230-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="78230-250">**lists**</span><span class="sxs-lookup"><span data-stu-id="78230-250">**lists**</span></span>         | <span data-ttu-id="78230-251">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="78230-251">Collection([list][])</span></span>             | <span data-ttu-id="78230-252">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="78230-252">The collection of lists under this site.</span></span>
| <span data-ttu-id="78230-253">**pages**</span><span class="sxs-lookup"><span data-stu-id="78230-253">**pages**</span></span>         | <span data-ttu-id="78230-254">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="78230-254">Collection([sitePage][])</span></span>         | <span data-ttu-id="78230-255">O conjunto de páginas na lista SitePages no site.</span><span class="sxs-lookup"><span data-stu-id="78230-255">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="78230-256">**permissões**</span><span class="sxs-lookup"><span data-stu-id="78230-256">**permissions**</span></span>   | <span data-ttu-id="78230-257">Coleção ([permissão][])</span><span class="sxs-lookup"><span data-stu-id="78230-257">Collection([permission][])</span></span>         | <span data-ttu-id="78230-258">As permissões associadas ao site.</span><span class="sxs-lookup"><span data-stu-id="78230-258">The permissions associated with the site.</span></span> <span data-ttu-id="78230-259">Anulável.</span><span class="sxs-lookup"><span data-stu-id="78230-259">Nullable.</span></span>
| <span data-ttu-id="78230-260">**sites**</span><span class="sxs-lookup"><span data-stu-id="78230-260">**sites**</span></span>         | <span data-ttu-id="78230-261">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="78230-261">Collection([site][])</span></span>             | <span data-ttu-id="78230-262">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="78230-262">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="78230-263">**externalColumns**</span><span class="sxs-lookup"><span data-stu-id="78230-263">**externalColumns**</span></span>     | <span data-ttu-id="78230-264">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="78230-264">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="78230-265">A coleção de definições de coluna disponíveis no site que são referenciadas nos sites na hierarquia pai do site atual.</span><span class="sxs-lookup"><span data-stu-id="78230-265">The collection of column definitions available in the site that are referenced from the sites in the parent hierarchy of the current site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="78230-278">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78230-278">JSON representation</span></span>

<span data-ttu-id="78230-279">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="78230-279">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="78230-280">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="78230-280">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
