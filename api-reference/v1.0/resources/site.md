---
author: JeremyKelley
ms.author: JeremyKelley
title: Recurso do site
description: O recurso do site fornece metadados e relações para um site do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1878b46f7738f440808960e43310b2d7606ee22f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533693"
---
# <a name="site-resource"></a><span data-ttu-id="22797-103">Recurso do site</span><span class="sxs-lookup"><span data-stu-id="22797-103">site resource</span></span>

<span data-ttu-id="22797-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22797-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22797-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="22797-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="22797-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="22797-106">Methods</span></span>

| <span data-ttu-id="22797-107">Método</span><span class="sxs-lookup"><span data-stu-id="22797-107">Method</span></span>                | <span data-ttu-id="22797-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="22797-108">Return type</span></span> | <span data-ttu-id="22797-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="22797-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="22797-110">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="22797-110">[Get root site][]</span></span>        | <span data-ttu-id="22797-111">site</span><span class="sxs-lookup"><span data-stu-id="22797-111">site</span></span> | <span data-ttu-id="22797-112">Acessar o site raiz do SharePoint dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="22797-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="22797-113">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="22797-113">[Get site][]</span></span>             | <span data-ttu-id="22797-114">site</span><span class="sxs-lookup"><span data-stu-id="22797-114">site</span></span> | <span data-ttu-id="22797-115">Acessar um site do sharePoint usando o siteId.</span><span class="sxs-lookup"><span data-stu-id="22797-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="22797-116">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="22797-116">[Get site by path][]</span></span>     | <span data-ttu-id="22797-117">site</span><span class="sxs-lookup"><span data-stu-id="22797-117">site</span></span> | <span data-ttu-id="22797-118">Acessar o site raiz do SharePoint com um caminho relativo.</span><span class="sxs-lookup"><span data-stu-id="22797-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="22797-119">[Obter site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="22797-119">[Get site for a group][]</span></span> | <span data-ttu-id="22797-120">site</span><span class="sxs-lookup"><span data-stu-id="22797-120">site</span></span> | <span data-ttu-id="22797-121">Acessar o site de equipe de um grupo.</span><span class="sxs-lookup"><span data-stu-id="22797-121">Access the team site for a group.</span></span>
| <span data-ttu-id="22797-122">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="22797-122">[Get analytics][]</span></span>              | <span data-ttu-id="22797-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="22797-123">[itemAnalytics][]</span></span> | <span data-ttu-id="22797-124">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="22797-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="22797-125">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="22797-125">[Get activities by interval][]</span></span> | <span data-ttu-id="22797-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="22797-126">[itemActivityStat][]</span></span> | <span data-ttu-id="22797-127">Obter uma coleção de **itemActivityStats** dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="22797-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="22797-128">[Pesquisar sites][]</span><span class="sxs-lookup"><span data-stu-id="22797-128">[Search for sites][]</span></span>     | <span data-ttu-id="22797-129">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="22797-129">collection of site</span></span> | <span data-ttu-id="22797-130">Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="22797-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>

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

## <a name="properties"></a><span data-ttu-id="22797-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22797-139">Properties</span></span>

| <span data-ttu-id="22797-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22797-140">Property</span></span>            | <span data-ttu-id="22797-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="22797-141">Type</span></span>                                | <span data-ttu-id="22797-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="22797-142">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="22797-143">**id**</span><span class="sxs-lookup"><span data-stu-id="22797-143">**id**</span></span>                   | <span data-ttu-id="22797-144">string</span><span class="sxs-lookup"><span data-stu-id="22797-144">string</span></span>                              | <span data-ttu-id="22797-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="22797-147">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="22797-147">**createdDateTime**</span></span>      | <span data-ttu-id="22797-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22797-148">DateTimeOffset</span></span>                      | <span data-ttu-id="22797-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="22797-151">**description**</span><span class="sxs-lookup"><span data-stu-id="22797-151">**description**</span></span>          | <span data-ttu-id="22797-152">string</span><span class="sxs-lookup"><span data-stu-id="22797-152">string</span></span>                              | <span data-ttu-id="22797-153">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="22797-153">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="22797-154">**displayName**</span><span class="sxs-lookup"><span data-stu-id="22797-154">**displayName**</span></span>          | <span data-ttu-id="22797-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22797-155">string</span></span>                              | <span data-ttu-id="22797-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="22797-158">**eTag**</span><span class="sxs-lookup"><span data-stu-id="22797-158">**eTag**</span></span>                 | <span data-ttu-id="22797-159">string</span><span class="sxs-lookup"><span data-stu-id="22797-159">string</span></span>                              | <span data-ttu-id="22797-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="22797-162">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="22797-162">**lastModifiedDateTime**</span></span> | <span data-ttu-id="22797-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22797-163">DateTimeOffset</span></span>                      | <span data-ttu-id="22797-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="22797-166">**name**</span><span class="sxs-lookup"><span data-stu-id="22797-166">**name**</span></span>                 | <span data-ttu-id="22797-167">string</span><span class="sxs-lookup"><span data-stu-id="22797-167">string</span></span>                              | <span data-ttu-id="22797-168">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="22797-168">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="22797-169">**root**</span><span class="sxs-lookup"><span data-stu-id="22797-169">**root**</span></span>                 | [<span data-ttu-id="22797-170">root</span><span class="sxs-lookup"><span data-stu-id="22797-170">root</span></span>](root.md)                     | <span data-ttu-id="22797-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="22797-173">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="22797-173">**sharepointIds**</span></span>        | [<span data-ttu-id="22797-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="22797-174">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="22797-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="22797-177">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="22797-177">**siteCollection**</span></span>       | [<span data-ttu-id="22797-178">siteCollection</span><span class="sxs-lookup"><span data-stu-id="22797-178">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="22797-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="22797-182">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="22797-182">**webUrl**</span></span>               | <span data-ttu-id="22797-183">string (url)</span><span class="sxs-lookup"><span data-stu-id="22797-183">string (url)</span></span>                        | <span data-ttu-id="22797-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="22797-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="22797-186">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="22797-186">Relationships</span></span>

| <span data-ttu-id="22797-187">Relação</span><span class="sxs-lookup"><span data-stu-id="22797-187">Relationship</span></span>      | <span data-ttu-id="22797-188">Tipo</span><span class="sxs-lookup"><span data-stu-id="22797-188">Type</span></span>                             | <span data-ttu-id="22797-189">Descrição</span><span class="sxs-lookup"><span data-stu-id="22797-189">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="22797-190">**analytics**</span><span class="sxs-lookup"><span data-stu-id="22797-190">**analytics**</span></span>     | <span data-ttu-id="22797-191">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="22797-191">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="22797-192">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="22797-192">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="22797-193">**columns**</span><span class="sxs-lookup"><span data-stu-id="22797-193">**columns**</span></span>       | <span data-ttu-id="22797-194">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="22797-194">Collection([columnDefinition][])</span></span> | <span data-ttu-id="22797-195">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="22797-195">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="22797-196">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="22797-196">**contentTypes**</span></span>  | <span data-ttu-id="22797-197">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="22797-197">Collection([contentType][])</span></span>      | <span data-ttu-id="22797-198">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="22797-198">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="22797-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="22797-199">**drive**</span></span>         | <span data-ttu-id="22797-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="22797-200">[drive][]</span></span>                        | <span data-ttu-id="22797-201">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="22797-201">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="22797-202">**drives**</span><span class="sxs-lookup"><span data-stu-id="22797-202">**drives**</span></span>        | <span data-ttu-id="22797-203">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="22797-203">Collection([drive][])</span></span>            | <span data-ttu-id="22797-204">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="22797-204">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="22797-205">**items**</span><span class="sxs-lookup"><span data-stu-id="22797-205">**items**</span></span>         | <span data-ttu-id="22797-206">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="22797-206">Collection([baseItem][])</span></span>         | <span data-ttu-id="22797-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="22797-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="22797-209">**lists**</span><span class="sxs-lookup"><span data-stu-id="22797-209">**lists**</span></span>         | <span data-ttu-id="22797-210">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="22797-210">Collection([list][])</span></span>             | <span data-ttu-id="22797-211">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="22797-211">The collection of lists under this site.</span></span>
| <span data-ttu-id="22797-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="22797-212">**sites**</span></span>         | <span data-ttu-id="22797-213">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="22797-213">Collection([site][])</span></span>             | <span data-ttu-id="22797-214">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="22797-214">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="22797-215">**onenote**</span><span class="sxs-lookup"><span data-stu-id="22797-215">**onenote**</span></span>       | <span data-ttu-id="22797-216">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="22797-216">[onenote][]</span></span>                      | <span data-ttu-id="22797-217">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="22797-217">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="22797-226">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22797-226">JSON representation</span></span>

<span data-ttu-id="22797-227">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="22797-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="22797-228">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="22797-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
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
