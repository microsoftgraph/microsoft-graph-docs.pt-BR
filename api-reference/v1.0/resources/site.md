---
author: JeremyKelley
ms.author: JeremyKelley
title: Recurso do site
description: O recurso do site fornece metadados e relações para um site do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f351ee2a9fe107ede3317a46789810ae2bf24b33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161366"
---
# <a name="site-resource"></a><span data-ttu-id="cd504-103">Recurso do site</span><span class="sxs-lookup"><span data-stu-id="cd504-103">site resource</span></span>

<span data-ttu-id="cd504-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd504-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd504-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cd504-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="cd504-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="cd504-106">Methods</span></span>

| <span data-ttu-id="cd504-107">Método</span><span class="sxs-lookup"><span data-stu-id="cd504-107">Method</span></span>                | <span data-ttu-id="cd504-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cd504-108">Return type</span></span> | <span data-ttu-id="cd504-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd504-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="cd504-110">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="cd504-110">[Get root site][]</span></span>        | <span data-ttu-id="cd504-111">site</span><span class="sxs-lookup"><span data-stu-id="cd504-111">site</span></span> | <span data-ttu-id="cd504-112">Acessar o site raiz do SharePoint dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="cd504-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="cd504-113">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="cd504-113">[Get site][]</span></span>             | <span data-ttu-id="cd504-114">site</span><span class="sxs-lookup"><span data-stu-id="cd504-114">site</span></span> | <span data-ttu-id="cd504-115">Acessar um site do sharePoint usando o siteId.</span><span class="sxs-lookup"><span data-stu-id="cd504-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="cd504-116">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="cd504-116">[Get site by path][]</span></span>     | <span data-ttu-id="cd504-117">site</span><span class="sxs-lookup"><span data-stu-id="cd504-117">site</span></span> | <span data-ttu-id="cd504-118">Acessar o site raiz do SharePoint com um caminho relativo.</span><span class="sxs-lookup"><span data-stu-id="cd504-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="cd504-119">[Obter site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="cd504-119">[Get site for a group][]</span></span> | <span data-ttu-id="cd504-120">site</span><span class="sxs-lookup"><span data-stu-id="cd504-120">site</span></span> | <span data-ttu-id="cd504-121">Acessar o site de equipe de um grupo.</span><span class="sxs-lookup"><span data-stu-id="cd504-121">Access the team site for a group.</span></span>
| <span data-ttu-id="cd504-122">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="cd504-122">[Get analytics][]</span></span>              | <span data-ttu-id="cd504-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="cd504-123">[itemAnalytics][]</span></span> | <span data-ttu-id="cd504-124">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="cd504-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="cd504-125">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="cd504-125">[Get activities by interval][]</span></span> | <span data-ttu-id="cd504-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="cd504-126">[itemActivityStat][]</span></span> | <span data-ttu-id="cd504-127">Obter uma coleção de **itemActivityStats** dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="cd504-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="cd504-128">[Pesquisar sites][]</span><span class="sxs-lookup"><span data-stu-id="cd504-128">[Search for sites][]</span></span>     | <span data-ttu-id="cd504-129">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="cd504-129">collection of site</span></span> | <span data-ttu-id="cd504-130">Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="cd504-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="cd504-131">[Seguir site][]</span><span class="sxs-lookup"><span data-stu-id="cd504-131">[Follow site][]</span></span>          | <span data-ttu-id="cd504-132">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="cd504-132">collection of site</span></span> | <span data-ttu-id="cd504-133">Seguir um ou vários sites de usuário.</span><span class="sxs-lookup"><span data-stu-id="cd504-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="cd504-134">[Deixar de seguir site][]</span><span class="sxs-lookup"><span data-stu-id="cd504-134">[Unfollow site][]</span></span>        | <span data-ttu-id="cd504-135">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="cd504-135">collection of site</span></span> | <span data-ttu-id="cd504-136">Seguir um ou vários sites de usuário.</span><span class="sxs-lookup"><span data-stu-id="cd504-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="cd504-137">[Listar sites seguidos][]</span><span class="sxs-lookup"><span data-stu-id="cd504-137">[List followed sites][]</span></span>  | <span data-ttu-id="cd504-138">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="cd504-138">collection of site</span></span> | <span data-ttu-id="cd504-139">Liste os sites que foram seguidos pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="cd504-139">List the sites that have been followed by the signed in user.</span></span>
| <span data-ttu-id="cd504-140">[Obter permissão][]</span><span class="sxs-lookup"><span data-stu-id="cd504-140">[Get permission][]</span></span>             | <span data-ttu-id="cd504-141">Obter /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="cd504-141">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="cd504-142">[Listar permissões][]</span><span class="sxs-lookup"><span data-stu-id="cd504-142">[List permissions][]</span></span>           | <span data-ttu-id="cd504-143">Obter /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="cd504-143">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="cd504-144">[Criar permissões][]</span><span class="sxs-lookup"><span data-stu-id="cd504-144">[Create permissions][]</span></span>         | <span data-ttu-id="cd504-145">Postar /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="cd504-145">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="cd504-146">[Excluir permissão][]</span><span class="sxs-lookup"><span data-stu-id="cd504-146">[Delete permission][]</span></span>         | <span data-ttu-id="cd504-147">Excluir /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="cd504-147">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="cd504-148">[Atualizar permissão][]</span><span class="sxs-lookup"><span data-stu-id="cd504-148">[Update permission][]</span></span>         | <span data-ttu-id="cd504-149">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="cd504-149">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Pesquisar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md
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

## <a name="properties"></a><span data-ttu-id="cd504-166">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd504-166">Properties</span></span>

| <span data-ttu-id="cd504-167">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd504-167">Property</span></span>            | <span data-ttu-id="cd504-168">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd504-168">Type</span></span>                                | <span data-ttu-id="cd504-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd504-169">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cd504-170">**id**</span><span class="sxs-lookup"><span data-stu-id="cd504-170">**id**</span></span>                   | <span data-ttu-id="cd504-171">string</span><span class="sxs-lookup"><span data-stu-id="cd504-171">string</span></span>                              | <span data-ttu-id="cd504-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="cd504-174">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="cd504-174">**createdDateTime**</span></span>      | <span data-ttu-id="cd504-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd504-175">DateTimeOffset</span></span>                      | <span data-ttu-id="cd504-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="cd504-178">**description**</span><span class="sxs-lookup"><span data-stu-id="cd504-178">**description**</span></span>          | <span data-ttu-id="cd504-179">string</span><span class="sxs-lookup"><span data-stu-id="cd504-179">string</span></span>                              | <span data-ttu-id="cd504-180">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="cd504-180">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="cd504-181">**displayName**</span><span class="sxs-lookup"><span data-stu-id="cd504-181">**displayName**</span></span>          | <span data-ttu-id="cd504-182">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cd504-182">string</span></span>                              | <span data-ttu-id="cd504-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="cd504-185">**eTag**</span><span class="sxs-lookup"><span data-stu-id="cd504-185">**eTag**</span></span>                 | <span data-ttu-id="cd504-186">string</span><span class="sxs-lookup"><span data-stu-id="cd504-186">string</span></span>                              | <span data-ttu-id="cd504-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="cd504-189">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cd504-189">**lastModifiedDateTime**</span></span> | <span data-ttu-id="cd504-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd504-190">DateTimeOffset</span></span>                      | <span data-ttu-id="cd504-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="cd504-193">**name**</span><span class="sxs-lookup"><span data-stu-id="cd504-193">**name**</span></span>                 | <span data-ttu-id="cd504-194">string</span><span class="sxs-lookup"><span data-stu-id="cd504-194">string</span></span>                              | <span data-ttu-id="cd504-195">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="cd504-195">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="cd504-196">**root**</span><span class="sxs-lookup"><span data-stu-id="cd504-196">**root**</span></span>                 | [<span data-ttu-id="cd504-197">root</span><span class="sxs-lookup"><span data-stu-id="cd504-197">root</span></span>](root.md)                     | <span data-ttu-id="cd504-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="cd504-200">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="cd504-200">**sharepointIds**</span></span>        | [<span data-ttu-id="cd504-201">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cd504-201">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="cd504-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="cd504-204">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="cd504-204">**siteCollection**</span></span>       | [<span data-ttu-id="cd504-205">siteCollection</span><span class="sxs-lookup"><span data-stu-id="cd504-205">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="cd504-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="cd504-209">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="cd504-209">**webUrl**</span></span>               | <span data-ttu-id="cd504-210">string (url)</span><span class="sxs-lookup"><span data-stu-id="cd504-210">string (url)</span></span>                        | <span data-ttu-id="cd504-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cd504-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="cd504-213">propriedade do id</span><span class="sxs-lookup"><span data-stu-id="cd504-213">id property</span></span>
<span data-ttu-id="cd504-214">Um **site** é identificado por um ID exclusivo que é composto pelos seguintes valores:</span><span class="sxs-lookup"><span data-stu-id="cd504-214">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="cd504-215">Hostname do conjunto de sites (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="cd504-215">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="cd504-216">ID exclusiva do conjunto de sites (GUID)</span><span class="sxs-lookup"><span data-stu-id="cd504-216">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="cd504-217">ID exclusiva do site (GUID)</span><span class="sxs-lookup"><span data-stu-id="cd504-217">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="cd504-218">O identificador `root` sempre faz referência ao site raiz de um determinado destino, como a seguir:</span><span class="sxs-lookup"><span data-stu-id="cd504-218">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="cd504-219">`/sites/root`: O site raiz do locatário.</span><span class="sxs-lookup"><span data-stu-id="cd504-219">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="cd504-220">`/groups/{group-id}/sites/root`: O site da equipe do grupo.</span><span class="sxs-lookup"><span data-stu-id="cd504-220">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="cd504-221">Relações</span><span class="sxs-lookup"><span data-stu-id="cd504-221">Relationships</span></span>

| <span data-ttu-id="cd504-222">Relação</span><span class="sxs-lookup"><span data-stu-id="cd504-222">Relationship</span></span>      | <span data-ttu-id="cd504-223">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd504-223">Type</span></span>                             | <span data-ttu-id="cd504-224">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd504-224">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="cd504-225">**analytics**</span><span class="sxs-lookup"><span data-stu-id="cd504-225">**analytics**</span></span>     | <span data-ttu-id="cd504-226">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="cd504-226">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="cd504-227">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="cd504-227">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="cd504-228">**columns**</span><span class="sxs-lookup"><span data-stu-id="cd504-228">**columns**</span></span>       | <span data-ttu-id="cd504-229">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="cd504-229">Collection([columnDefinition][])</span></span> | <span data-ttu-id="cd504-230">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="cd504-230">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="cd504-231">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="cd504-231">**contentTypes**</span></span>  | <span data-ttu-id="cd504-232">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="cd504-232">Collection([contentType][])</span></span>      | <span data-ttu-id="cd504-233">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="cd504-233">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="cd504-234">**drive**</span><span class="sxs-lookup"><span data-stu-id="cd504-234">**drive**</span></span>         | <span data-ttu-id="cd504-235">[drive][]</span><span class="sxs-lookup"><span data-stu-id="cd504-235">[drive][]</span></span>                        | <span data-ttu-id="cd504-236">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="cd504-236">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="cd504-237">**drives**</span><span class="sxs-lookup"><span data-stu-id="cd504-237">**drives**</span></span>        | <span data-ttu-id="cd504-238">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="cd504-238">Collection([drive][])</span></span>            | <span data-ttu-id="cd504-239">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="cd504-239">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="cd504-240">**items**</span><span class="sxs-lookup"><span data-stu-id="cd504-240">**items**</span></span>         | <span data-ttu-id="cd504-241">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="cd504-241">Collection([baseItem][])</span></span>         | <span data-ttu-id="cd504-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="cd504-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="cd504-244">**lists**</span><span class="sxs-lookup"><span data-stu-id="cd504-244">**lists**</span></span>         | <span data-ttu-id="cd504-245">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="cd504-245">Collection([list][])</span></span>             | <span data-ttu-id="cd504-246">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="cd504-246">The collection of lists under this site.</span></span>
| <span data-ttu-id="cd504-247">**Permissões**</span><span class="sxs-lookup"><span data-stu-id="cd504-247">**permissions**</span></span>   | <span data-ttu-id="cd504-248">Coleção ([permissão][])</span><span class="sxs-lookup"><span data-stu-id="cd504-248">Collection([permission][])</span></span>         | <span data-ttu-id="cd504-249">As permissões associadas ao site.</span><span class="sxs-lookup"><span data-stu-id="cd504-249">The permissions associated with the site.</span></span> <span data-ttu-id="cd504-250">Anulável.</span><span class="sxs-lookup"><span data-stu-id="cd504-250">Nullable.</span></span>
| <span data-ttu-id="cd504-251">**sites**</span><span class="sxs-lookup"><span data-stu-id="cd504-251">**sites**</span></span>         | <span data-ttu-id="cd504-252">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="cd504-252">Collection([site][])</span></span>             | <span data-ttu-id="cd504-253">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="cd504-253">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="cd504-254">**onenote**</span><span class="sxs-lookup"><span data-stu-id="cd504-254">**onenote**</span></span>       | <span data-ttu-id="cd504-255">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="cd504-255">[onenote][]</span></span>                      | <span data-ttu-id="cd504-256">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="cd504-256">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permissão]: permission.md
[permission]: permission.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="cd504-266">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd504-266">JSON representation</span></span>

<span data-ttu-id="cd504-267">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="cd504-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="cd504-268">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="cd504-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
