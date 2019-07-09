---
author: JeremyKelley
ms.author: JeremyKelley
title: Recurso do site
description: O recurso do site fornece metadados e relações para um site do SharePoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 40add99dfbeee28d82b3d02def833497c01385df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968846"
---
# <a name="site-resource"></a><span data-ttu-id="41045-103">Recurso do site</span><span class="sxs-lookup"><span data-stu-id="41045-103">Site resource</span></span>

<span data-ttu-id="41045-104">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="41045-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="41045-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="41045-105">Methods</span></span>

| <span data-ttu-id="41045-106">Método</span><span class="sxs-lookup"><span data-stu-id="41045-106">Method</span></span>                | <span data-ttu-id="41045-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="41045-107">Return type</span></span> | <span data-ttu-id="41045-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="41045-108">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="41045-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="41045-109">[Get root site][]</span></span>        | <span data-ttu-id="41045-110">site</span><span class="sxs-lookup"><span data-stu-id="41045-110">Site</span></span> | <span data-ttu-id="41045-111">Acessar o site raiz do SharePoint dentro de um locatário.</span><span class="sxs-lookup"><span data-stu-id="41045-111">To access the root SharePoint site within a tenant:</span></span>
| <span data-ttu-id="41045-112">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="41045-112">[Get site][]</span></span>             | <span data-ttu-id="41045-113">site</span><span class="sxs-lookup"><span data-stu-id="41045-113">Site</span></span> | <span data-ttu-id="41045-114">Acessar um site do sharePoint usando o siteId.</span><span class="sxs-lookup"><span data-stu-id="41045-114">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="41045-115">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="41045-115">[Get site by path][]</span></span>     | <span data-ttu-id="41045-116">site</span><span class="sxs-lookup"><span data-stu-id="41045-116">Site</span></span> | <span data-ttu-id="41045-117">Acessar o site raiz do SharePoint com um caminho relativo.</span><span class="sxs-lookup"><span data-stu-id="41045-117">To access the root SharePoint site with a relative path:</span></span>
| <span data-ttu-id="41045-118">[Obter site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="41045-118">[Get site for a group][]</span></span> | <span data-ttu-id="41045-119">site</span><span class="sxs-lookup"><span data-stu-id="41045-119">Site</span></span> | <span data-ttu-id="41045-120">Acessar o site de equipe de um grupo.</span><span class="sxs-lookup"><span data-stu-id="41045-120">To access the team site for a group:</span></span>
| <span data-ttu-id="41045-121">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="41045-121">[Get analytics][]</span></span>              | <span data-ttu-id="41045-122">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="41045-122">[itemAnalytics][]</span></span> | <span data-ttu-id="41045-123">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="41045-123">Get analytics for this resource.</span></span> 
| <span data-ttu-id="41045-124">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="41045-124">[Get activities by interval][]</span></span> | <span data-ttu-id="41045-125">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="41045-125">[itemActivityStat][]</span></span> | <span data-ttu-id="41045-126">Obter uma coleção de **itemActivityStats** dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="41045-126">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="41045-127">[Pesquisar sites][]</span><span class="sxs-lookup"><span data-stu-id="41045-127">[Search for sites][]</span></span>     | <span data-ttu-id="41045-128">coleção de sites</span><span class="sxs-lookup"><span data-stu-id="41045-128">Specifies a collection of site templates.</span></span> | <span data-ttu-id="41045-129">Pesquise num locatário do SharePoint por sites que correspondam a palavras-chave fornecidas.</span><span class="sxs-lookup"><span data-stu-id="41045-129">Search across a SharePoint tenant for sites that match provided keywords.</span></span>

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

## <a name="properties"></a><span data-ttu-id="41045-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41045-138">Properties</span></span>

| <span data-ttu-id="41045-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41045-139">Property</span></span>            | <span data-ttu-id="41045-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="41045-140">Type</span></span>                                | <span data-ttu-id="41045-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="41045-141">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="41045-142">**id**</span><span class="sxs-lookup"><span data-stu-id="41045-142">**id**</span></span>                   | <span data-ttu-id="41045-143">string</span><span class="sxs-lookup"><span data-stu-id="41045-143">string</span></span>                              | <span data-ttu-id="41045-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="41045-146">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="41045-146">**createdDateTime**</span></span>      | <span data-ttu-id="41045-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41045-147">DateTimeOffset</span></span>                      | <span data-ttu-id="41045-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="41045-150">**description**</span><span class="sxs-lookup"><span data-stu-id="41045-150">**description**</span></span>          | <span data-ttu-id="41045-151">string</span><span class="sxs-lookup"><span data-stu-id="41045-151">string</span></span>                              | <span data-ttu-id="41045-152">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="41045-152">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="41045-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="41045-153">**displayName**</span></span>          | <span data-ttu-id="41045-154">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="41045-154">string</span></span>                              | <span data-ttu-id="41045-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="41045-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="41045-157">**eTag**</span></span>                 | <span data-ttu-id="41045-158">string</span><span class="sxs-lookup"><span data-stu-id="41045-158">string</span></span>                              | <span data-ttu-id="41045-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="41045-161">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="41045-161">**lastModifiedDateTime**</span></span> | <span data-ttu-id="41045-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41045-162">DateTimeOffset</span></span>                      | <span data-ttu-id="41045-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="41045-165">**name**</span><span class="sxs-lookup"><span data-stu-id="41045-165">**name**</span></span>                 | <span data-ttu-id="41045-166">string</span><span class="sxs-lookup"><span data-stu-id="41045-166">string</span></span>                              | <span data-ttu-id="41045-167">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="41045-167">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="41045-168">**root**</span><span class="sxs-lookup"><span data-stu-id="41045-168">**root**</span></span>                 | [<span data-ttu-id="41045-169">root</span><span class="sxs-lookup"><span data-stu-id="41045-169">root</span></span>](root.md)                     | <span data-ttu-id="41045-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="41045-172">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="41045-172">**sharepointIds**</span></span>        | [<span data-ttu-id="41045-173">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="41045-173">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="41045-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="41045-176">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="41045-176">**siteCollection**</span></span>       | [<span data-ttu-id="41045-177">siteCollection</span><span class="sxs-lookup"><span data-stu-id="41045-177">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="41045-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="41045-181">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="41045-181">**webUrl**</span></span>               | <span data-ttu-id="41045-182">string (url)</span><span class="sxs-lookup"><span data-stu-id="41045-182">string (url)</span></span>                        | <span data-ttu-id="41045-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="41045-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="41045-185">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="41045-185">Relationships</span></span>

| <span data-ttu-id="41045-186">Relação</span><span class="sxs-lookup"><span data-stu-id="41045-186">Relationship</span></span>      | <span data-ttu-id="41045-187">Tipo</span><span class="sxs-lookup"><span data-stu-id="41045-187">Type</span></span>                             | <span data-ttu-id="41045-188">Descrição</span><span class="sxs-lookup"><span data-stu-id="41045-188">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="41045-189">**analytics**</span><span class="sxs-lookup"><span data-stu-id="41045-189">**analytics**</span></span>     | <span data-ttu-id="41045-190">[itemAnalytics][] resource</span><span class="sxs-lookup"><span data-stu-id="41045-190">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="41045-191">Análise sobre as atividades de modo de exibição que ocorreram no site.</span><span class="sxs-lookup"><span data-stu-id="41045-191">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="41045-192">**columns**</span><span class="sxs-lookup"><span data-stu-id="41045-192">**columns**</span></span>       | <span data-ttu-id="41045-193">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="41045-193">Collection([columnDefinition][])</span></span> | <span data-ttu-id="41045-194">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="41045-194">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="41045-195">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="41045-195">**contentTypes**</span></span>  | <span data-ttu-id="41045-196">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="41045-196">Collection([contentType][])</span></span>      | <span data-ttu-id="41045-197">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="41045-197">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="41045-198">**drive**</span><span class="sxs-lookup"><span data-stu-id="41045-198">**drive**</span></span>         | <span data-ttu-id="41045-199">[drive][]</span><span class="sxs-lookup"><span data-stu-id="41045-199">[drive][]</span></span>                        | <span data-ttu-id="41045-200">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="41045-200">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="41045-201">**drives**</span><span class="sxs-lookup"><span data-stu-id="41045-201">**drives**</span></span>        | <span data-ttu-id="41045-202">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="41045-202">Collection([drive][])</span></span>            | <span data-ttu-id="41045-203">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="41045-203">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="41045-204">**items**</span><span class="sxs-lookup"><span data-stu-id="41045-204">**items**</span></span>         | <span data-ttu-id="41045-205">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="41045-205">Collection([baseItem][])</span></span>         | <span data-ttu-id="41045-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="41045-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="41045-208">**lists**</span><span class="sxs-lookup"><span data-stu-id="41045-208">**lists**</span></span>         | <span data-ttu-id="41045-209">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="41045-209">Collection([list][])</span></span>             | <span data-ttu-id="41045-210">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="41045-210">The collection of lists under this site.</span></span>
| <span data-ttu-id="41045-211">**sites**</span><span class="sxs-lookup"><span data-stu-id="41045-211">**sites**</span></span>         | <span data-ttu-id="41045-212">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="41045-212">Collection([site][])</span></span>             | <span data-ttu-id="41045-213">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="41045-213">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="41045-214">**onenote**</span><span class="sxs-lookup"><span data-stu-id="41045-214">**onenote**</span></span>       | <span data-ttu-id="41045-215">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="41045-215">[onenote][]</span></span>                      | <span data-ttu-id="41045-216">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="41045-216">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="41045-225">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41045-225">JSON representation</span></span>

<span data-ttu-id="41045-226">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="41045-226">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="41045-227">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="41045-227">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
