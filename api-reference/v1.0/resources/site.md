---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: ae8962dfa38c3c6f3e06ccb687eb42a4a8262f1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007538"
---
# <a name="site-resource"></a><span data-ttu-id="ef431-102">Recurso site</span><span class="sxs-lookup"><span data-stu-id="ef431-102">Site resource</span></span>

<span data-ttu-id="ef431-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ef431-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="ef431-104">Tarefas</span><span class="sxs-lookup"><span data-stu-id="ef431-104">Tasks</span></span>

<span data-ttu-id="ef431-105">Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="ef431-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="ef431-106">Nome da tarefa</span><span class="sxs-lookup"><span data-stu-id="ef431-106">Task name</span></span>                | <span data-ttu-id="ef431-107">Exemplo de Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef431-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="ef431-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="ef431-108">[Get root site][]</span></span>        | <span data-ttu-id="ef431-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ef431-109">GET /sites/root</span></span>
| <span data-ttu-id="ef431-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="ef431-110">[Get site][]</span></span>             | <span data-ttu-id="ef431-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ef431-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ef431-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="ef431-112">[Get site by path][]</span></span>     | <span data-ttu-id="ef431-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ef431-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ef431-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="ef431-114">[Get site for a group][]</span></span> | <span data-ttu-id="ef431-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ef431-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ef431-116">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="ef431-116">[Search for sites][]</span></span>     | <span data-ttu-id="ef431-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ef431-117">GET /sites?search={query}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ef431-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef431-123">JSON representation</span></span>

<span data-ttu-id="ef431-124">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="ef431-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ef431-125">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="ef431-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ef431-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef431-126">Properties</span></span>

| <span data-ttu-id="ef431-127">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ef431-127">Property name</span></span>            | <span data-ttu-id="ef431-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef431-128">Type</span></span>                                | <span data-ttu-id="ef431-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef431-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ef431-130">**id**</span><span class="sxs-lookup"><span data-stu-id="ef431-130">**id**</span></span>                   | <span data-ttu-id="ef431-131">string</span><span class="sxs-lookup"><span data-stu-id="ef431-131">string</span></span>                              | <span data-ttu-id="ef431-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="ef431-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef431-134">**createdDateTime**</span></span>      | <span data-ttu-id="ef431-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef431-135">DateTimeOffset</span></span>                      | <span data-ttu-id="ef431-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="ef431-138">**description**</span><span class="sxs-lookup"><span data-stu-id="ef431-138">**description**</span></span>          | <span data-ttu-id="ef431-139">string</span><span class="sxs-lookup"><span data-stu-id="ef431-139">string</span></span>                              | <span data-ttu-id="ef431-140">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="ef431-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="ef431-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ef431-141">**displayName**</span></span>          | <span data-ttu-id="ef431-142">string</span><span class="sxs-lookup"><span data-stu-id="ef431-142">string</span></span>                              | <span data-ttu-id="ef431-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="ef431-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ef431-145">**eTag**</span></span>                 | <span data-ttu-id="ef431-146">string</span><span class="sxs-lookup"><span data-stu-id="ef431-146">string</span></span>                              | <span data-ttu-id="ef431-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ef431-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef431-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ef431-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef431-150">DateTimeOffset</span></span>                      | <span data-ttu-id="ef431-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="ef431-153">**name**</span><span class="sxs-lookup"><span data-stu-id="ef431-153">**name**</span></span>                 | <span data-ttu-id="ef431-154">string</span><span class="sxs-lookup"><span data-stu-id="ef431-154">string</span></span>                              | <span data-ttu-id="ef431-155">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="ef431-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="ef431-156">**root**</span><span class="sxs-lookup"><span data-stu-id="ef431-156">**root**</span></span>                 | [<span data-ttu-id="ef431-157">root</span><span class="sxs-lookup"><span data-stu-id="ef431-157">root</span></span>](root.md)                     | <span data-ttu-id="ef431-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="ef431-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ef431-160">**sharepointIds**</span></span>        | [<span data-ttu-id="ef431-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ef431-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="ef431-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="ef431-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ef431-164">**siteCollection**</span></span>       | [<span data-ttu-id="ef431-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="ef431-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="ef431-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="ef431-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ef431-169">**webUrl**</span></span>               | <span data-ttu-id="ef431-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="ef431-170">string (url)</span></span>                        | <span data-ttu-id="ef431-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef431-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="ef431-173">Relações</span><span class="sxs-lookup"><span data-stu-id="ef431-173">Relationships</span></span>

| <span data-ttu-id="ef431-174">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="ef431-174">Relationship name</span></span> | <span data-ttu-id="ef431-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef431-175">Type</span></span>                             | <span data-ttu-id="ef431-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef431-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ef431-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="ef431-177">**columns**</span></span>       | <span data-ttu-id="ef431-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ef431-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ef431-179">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="ef431-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ef431-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ef431-180">**contentTypes**</span></span>  | <span data-ttu-id="ef431-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ef431-181">Collection([contentType][])</span></span>      | <span data-ttu-id="ef431-182">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="ef431-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ef431-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="ef431-183">**drive**</span></span>         | <span data-ttu-id="ef431-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ef431-184">[drive][]</span></span>                        | <span data-ttu-id="ef431-185">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="ef431-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ef431-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="ef431-186">**drives**</span></span>        | <span data-ttu-id="ef431-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="ef431-187">Collection([drive][])</span></span>            | <span data-ttu-id="ef431-188">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="ef431-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ef431-189">**items**</span><span class="sxs-lookup"><span data-stu-id="ef431-189">**items**</span></span>         | <span data-ttu-id="ef431-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ef431-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="ef431-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="ef431-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ef431-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="ef431-193">**lists**</span></span>         | <span data-ttu-id="ef431-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ef431-194">Collection([list][])</span></span>             | <span data-ttu-id="ef431-195">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="ef431-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="ef431-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="ef431-196">**sites**</span></span>         | <span data-ttu-id="ef431-197">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="ef431-197">Collection([site][])</span></span>             | <span data-ttu-id="ef431-198">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="ef431-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="ef431-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="ef431-199">**onenote**</span></span>       | <span data-ttu-id="ef431-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="ef431-200">[onenote][]</span></span>                      | <span data-ttu-id="ef431-201">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="ef431-201">Calls the OneNote service for notebook related operations.</span></span>

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
