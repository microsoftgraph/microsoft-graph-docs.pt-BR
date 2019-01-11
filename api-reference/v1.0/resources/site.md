---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.openlocfilehash: bdb8387c49e76e3f326cffe595397e6277d40738
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821095"
---
# <a name="site-resource"></a><span data-ttu-id="fbc52-102">Recurso site</span><span class="sxs-lookup"><span data-stu-id="fbc52-102">Site resource</span></span>

<span data-ttu-id="fbc52-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fbc52-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="fbc52-104">Tarefas</span><span class="sxs-lookup"><span data-stu-id="fbc52-104">Tasks</span></span>

<span data-ttu-id="fbc52-105">Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="fbc52-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="fbc52-106">Nome da tarefa</span><span class="sxs-lookup"><span data-stu-id="fbc52-106">Task name</span></span>                | <span data-ttu-id="fbc52-107">Exemplo de Solicitação</span><span class="sxs-lookup"><span data-stu-id="fbc52-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="fbc52-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-108">[Get root site][]</span></span>        | <span data-ttu-id="fbc52-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="fbc52-109">GET /sites/root</span></span>
| <span data-ttu-id="fbc52-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-110">[Get site][]</span></span>             | <span data-ttu-id="fbc52-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="fbc52-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="fbc52-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-112">[Get site by path][]</span></span>     | <span data-ttu-id="fbc52-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="fbc52-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="fbc52-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-114">[Get site for a group][]</span></span> | <span data-ttu-id="fbc52-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="fbc52-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="fbc52-116">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-116">[Search for sites][]</span></span>     | <span data-ttu-id="fbc52-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="fbc52-117">GET /sites?search={query}</span></span>

[Obter site]: ../api/site-get.md
[Get site]: ../api/site-get.md
[Obter site raiz]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[Obter site por caminho]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[Obter o site para um grupo]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[Procurar sites]: ../api/site-search.md
[Search for sites]: ../api/site-search.md

## <a name="json-representation"></a><span data-ttu-id="fbc52-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc52-123">JSON representation</span></span>

<span data-ttu-id="fbc52-124">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="fbc52-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="fbc52-125">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc52-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fbc52-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc52-126">Properties</span></span>

| <span data-ttu-id="fbc52-127">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc52-127">Property name</span></span>            | <span data-ttu-id="fbc52-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc52-128">Type</span></span>                                | <span data-ttu-id="fbc52-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc52-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fbc52-130">**id**</span><span class="sxs-lookup"><span data-stu-id="fbc52-130">**id**</span></span>                   | <span data-ttu-id="fbc52-131">string</span><span class="sxs-lookup"><span data-stu-id="fbc52-131">string</span></span>                              | <span data-ttu-id="fbc52-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="fbc52-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="fbc52-134">**createdDateTime**</span></span>      | <span data-ttu-id="fbc52-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc52-135">DateTimeOffset</span></span>                      | <span data-ttu-id="fbc52-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="fbc52-138">**description**</span><span class="sxs-lookup"><span data-stu-id="fbc52-138">**description**</span></span>          | <span data-ttu-id="fbc52-139">string</span><span class="sxs-lookup"><span data-stu-id="fbc52-139">string</span></span>                              | <span data-ttu-id="fbc52-140">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="fbc52-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="fbc52-141">**displayName**</span></span>          | <span data-ttu-id="fbc52-142">string</span><span class="sxs-lookup"><span data-stu-id="fbc52-142">string</span></span>                              | <span data-ttu-id="fbc52-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="fbc52-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="fbc52-145">**eTag**</span></span>                 | <span data-ttu-id="fbc52-146">string</span><span class="sxs-lookup"><span data-stu-id="fbc52-146">string</span></span>                              | <span data-ttu-id="fbc52-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="fbc52-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fbc52-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="fbc52-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbc52-150">DateTimeOffset</span></span>                      | <span data-ttu-id="fbc52-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="fbc52-153">**name**</span><span class="sxs-lookup"><span data-stu-id="fbc52-153">**name**</span></span>                 | <span data-ttu-id="fbc52-154">string</span><span class="sxs-lookup"><span data-stu-id="fbc52-154">string</span></span>                              | <span data-ttu-id="fbc52-155">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="fbc52-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="fbc52-156">**root**</span><span class="sxs-lookup"><span data-stu-id="fbc52-156">**root**</span></span>                 | [<span data-ttu-id="fbc52-157">root</span><span class="sxs-lookup"><span data-stu-id="fbc52-157">root</span></span>](root.md)                     | <span data-ttu-id="fbc52-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="fbc52-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="fbc52-160">**sharepointIds**</span></span>        | [<span data-ttu-id="fbc52-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="fbc52-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="fbc52-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="fbc52-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="fbc52-164">**siteCollection**</span></span>       | [<span data-ttu-id="fbc52-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="fbc52-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="fbc52-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="fbc52-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="fbc52-169">**webUrl**</span></span>               | <span data-ttu-id="fbc52-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="fbc52-170">string (url)</span></span>                        | <span data-ttu-id="fbc52-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="fbc52-173">Relações</span><span class="sxs-lookup"><span data-stu-id="fbc52-173">Relationships</span></span>

| <span data-ttu-id="fbc52-174">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fbc52-174">Relationship name</span></span> | <span data-ttu-id="fbc52-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc52-175">Type</span></span>                             | <span data-ttu-id="fbc52-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc52-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="fbc52-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="fbc52-177">**columns**</span></span>       | <span data-ttu-id="fbc52-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="fbc52-179">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="fbc52-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="fbc52-180">**contentTypes**</span></span>  | <span data-ttu-id="fbc52-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-181">Collection([contentType][])</span></span>      | <span data-ttu-id="fbc52-182">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="fbc52-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="fbc52-183">**drive**</span></span>         | <span data-ttu-id="fbc52-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-184">[drive][]</span></span>                        | <span data-ttu-id="fbc52-185">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="fbc52-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="fbc52-186">**drives**</span></span>        | <span data-ttu-id="fbc52-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-187">Collection([drive][])</span></span>            | <span data-ttu-id="fbc52-188">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="fbc52-189">**items**</span><span class="sxs-lookup"><span data-stu-id="fbc52-189">**items**</span></span>         | <span data-ttu-id="fbc52-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="fbc52-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="fbc52-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="fbc52-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="fbc52-193">**lists**</span></span>         | <span data-ttu-id="fbc52-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-194">Collection([list][])</span></span>             | <span data-ttu-id="fbc52-195">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="fbc52-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="fbc52-196">**sites**</span></span>         | <span data-ttu-id="fbc52-197">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="fbc52-197">Collection([site][])</span></span>             | <span data-ttu-id="fbc52-198">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="fbc52-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="fbc52-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="fbc52-199">**onenote**</span></span>       | <span data-ttu-id="fbc52-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="fbc52-200">[onenote][]</span></span>                      | <span data-ttu-id="fbc52-201">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="fbc52-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
