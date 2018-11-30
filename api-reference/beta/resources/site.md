---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: d18487d9932227df0ce2de3320fcb71ce94ca735
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038903"
---
# <a name="site-resource-type"></a><span data-ttu-id="ad64a-102">tipo de recurso de site</span><span class="sxs-lookup"><span data-stu-id="ad64a-102">site resource type</span></span>

> <span data-ttu-id="ad64a-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ad64a-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad64a-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ad64a-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ad64a-105">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ad64a-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ad64a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ad64a-106">Methods</span></span>

| <span data-ttu-id="ad64a-107">Método</span><span class="sxs-lookup"><span data-stu-id="ad64a-107">Method</span></span>                         | <span data-ttu-id="ad64a-108">Caminho REST</span><span class="sxs-lookup"><span data-stu-id="ad64a-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="ad64a-109">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-109">[Get root site][]</span></span>              | <span data-ttu-id="ad64a-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ad64a-110">GET /sites/root</span></span>
| <span data-ttu-id="ad64a-111">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-111">[Get site][]</span></span>                   | <span data-ttu-id="ad64a-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ad64a-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ad64a-113">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-113">[Get site by path][]</span></span>           | <span data-ttu-id="ad64a-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ad64a-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ad64a-115">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-115">[Get site for a group][]</span></span>       | <span data-ttu-id="ad64a-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ad64a-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ad64a-117">[Obtenha a análise][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-117">[Get analytics][]</span></span>              | <span data-ttu-id="ad64a-118">GET /sites/ {site-id} / análise</span><span class="sxs-lookup"><span data-stu-id="ad64a-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="ad64a-119">[Fazer atividades pelo intervalo][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-119">[Get activities by interval][]</span></span> | <span data-ttu-id="ad64a-120">GET /sites/ {site-id} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ad64a-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ad64a-121">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-121">[List pages][]</span></span>                 | <span data-ttu-id="ad64a-122">GET /sites/ {site-id} / páginas</span><span class="sxs-lookup"><span data-stu-id="ad64a-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="ad64a-123">[Lista de sites de raiz][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-123">[List root sites][]</span></span>            | <span data-ttu-id="ad64a-124">GET /sites? filtro = raiz ne nulo & Selecionar = siteCollection, webUrl</span><span class="sxs-lookup"><span data-stu-id="ad64a-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="ad64a-125">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-125">[Search for sites][]</span></span>           | <span data-ttu-id="ad64a-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ad64a-126">GET /sites?search={query}</span></span>

[Obter site]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Obtenha a análise]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Fazer atividades pelo intervalo]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Lista de sites de raiz]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[Procurar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="ad64a-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad64a-136">Properties</span></span>

| <span data-ttu-id="ad64a-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ad64a-137">Property name</span></span>            | <span data-ttu-id="ad64a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad64a-138">Type</span></span>               | <span data-ttu-id="ad64a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad64a-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="ad64a-140">**id**</span><span class="sxs-lookup"><span data-stu-id="ad64a-140">**id**</span></span>                   | <span data-ttu-id="ad64a-141">string</span><span class="sxs-lookup"><span data-stu-id="ad64a-141">string</span></span>             | <span data-ttu-id="ad64a-p102">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ad64a-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ad64a-144">**createdDateTime**</span></span>      | <span data-ttu-id="ad64a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad64a-145">DateTimeOffset</span></span>     | <span data-ttu-id="ad64a-p103">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ad64a-148">**description**</span><span class="sxs-lookup"><span data-stu-id="ad64a-148">**description**</span></span>          | <span data-ttu-id="ad64a-149">string</span><span class="sxs-lookup"><span data-stu-id="ad64a-149">string</span></span>             | <span data-ttu-id="ad64a-150">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="ad64a-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ad64a-151">**eTag**</span></span>                 | <span data-ttu-id="ad64a-152">string</span><span class="sxs-lookup"><span data-stu-id="ad64a-152">string</span></span>             | <span data-ttu-id="ad64a-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ad64a-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ad64a-155">**displayName**</span></span>          | <span data-ttu-id="ad64a-156">string</span><span class="sxs-lookup"><span data-stu-id="ad64a-156">string</span></span>             | <span data-ttu-id="ad64a-p105">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="ad64a-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ad64a-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ad64a-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad64a-160">DateTimeOffset</span></span>     | <span data-ttu-id="ad64a-p106">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ad64a-163">**name**</span><span class="sxs-lookup"><span data-stu-id="ad64a-163">**name**</span></span>                 | <span data-ttu-id="ad64a-164">string</span><span class="sxs-lookup"><span data-stu-id="ad64a-164">string</span></span>             | <span data-ttu-id="ad64a-165">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="ad64a-165">The name / title of the item.</span></span>
| <span data-ttu-id="ad64a-166">**root**</span><span class="sxs-lookup"><span data-stu-id="ad64a-166">**root**</span></span>                 | <span data-ttu-id="ad64a-167">[root][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-167">[root][]</span></span>           | <span data-ttu-id="ad64a-p107">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="ad64a-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ad64a-170">**sharepointIds**</span></span>        | <span data-ttu-id="ad64a-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-171">[sharepointIds][]</span></span>  | <span data-ttu-id="ad64a-p108">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ad64a-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ad64a-174">**siteCollection**</span></span>       | <span data-ttu-id="ad64a-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-175">[siteCollection][]</span></span> | <span data-ttu-id="ad64a-p109">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="ad64a-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ad64a-179">**webUrl**</span></span>               | <span data-ttu-id="ad64a-180">string (url)</span><span class="sxs-lookup"><span data-stu-id="ad64a-180">string (url)</span></span>       | <span data-ttu-id="ad64a-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ad64a-183">Relações</span><span class="sxs-lookup"><span data-stu-id="ad64a-183">Relationships</span></span>

| <span data-ttu-id="ad64a-184">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ad64a-184">Relationship name</span></span> | <span data-ttu-id="ad64a-185">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad64a-185">Type</span></span>                             | <span data-ttu-id="ad64a-186">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad64a-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ad64a-187">**análise**</span><span class="sxs-lookup"><span data-stu-id="ad64a-187">**analytics**</span></span>     | <span data-ttu-id="ad64a-188">recurso de [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ad64a-189">Análise sobre as atividades de modo de exibição que foram realizada neste site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ad64a-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="ad64a-190">**columns**</span></span>       | <span data-ttu-id="ad64a-191">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ad64a-192">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ad64a-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ad64a-193">**contentTypes**</span></span>  | <span data-ttu-id="ad64a-194">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-194">Collection([contentType][])</span></span>      | <span data-ttu-id="ad64a-195">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ad64a-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="ad64a-196">**drive**</span></span>         | <span data-ttu-id="ad64a-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ad64a-197">[drive][]</span></span>                        | <span data-ttu-id="ad64a-198">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ad64a-199">**drives**</span><span class="sxs-lookup"><span data-stu-id="ad64a-199">**drives**</span></span>        | <span data-ttu-id="ad64a-200">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-200">Collection([drive][])</span></span>            | <span data-ttu-id="ad64a-201">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ad64a-202">**items**</span><span class="sxs-lookup"><span data-stu-id="ad64a-202">**items**</span></span>         | <span data-ttu-id="ad64a-203">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="ad64a-p111">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="ad64a-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ad64a-206">**lists**</span><span class="sxs-lookup"><span data-stu-id="ad64a-206">**lists**</span></span>         | <span data-ttu-id="ad64a-207">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-207">Collection([list][])</span></span>             | <span data-ttu-id="ad64a-208">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="ad64a-209">**páginas**</span><span class="sxs-lookup"><span data-stu-id="ad64a-209">**pages**</span></span>         | <span data-ttu-id="ad64a-210">Coleção ([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="ad64a-211">A coleção de páginas na lista SitePages neste site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="ad64a-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="ad64a-212">**sites**</span></span>         | <span data-ttu-id="ad64a-213">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ad64a-213">Collection([site][])</span></span>             | <span data-ttu-id="ad64a-214">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="ad64a-214">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[lista]: list.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="ad64a-226">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad64a-226">JSON representation</span></span>

<span data-ttu-id="ad64a-227">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="ad64a-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ad64a-228">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="ad64a-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
