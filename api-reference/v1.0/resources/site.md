---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: cd0631d8426dffa6ea731fabe024a1028e080f1c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937009"
---
# <a name="site-resource"></a><span data-ttu-id="fd7e4-102">Recurso site</span><span class="sxs-lookup"><span data-stu-id="fd7e4-102">Site resource</span></span>

<span data-ttu-id="fd7e4-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="fd7e4-104">Tarefas</span><span class="sxs-lookup"><span data-stu-id="fd7e4-104">Tasks</span></span>

<span data-ttu-id="fd7e4-105">Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="fd7e4-106">Nome da tarefa</span><span class="sxs-lookup"><span data-stu-id="fd7e4-106">Task name</span></span>                | <span data-ttu-id="fd7e4-107">Exemplo de Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd7e4-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="fd7e4-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-108">[Get root site][]</span></span>        | <span data-ttu-id="fd7e4-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="fd7e4-109">GET /sites/root</span></span>
| <span data-ttu-id="fd7e4-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-110">[Get site][]</span></span>             | <span data-ttu-id="fd7e4-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="fd7e4-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="fd7e4-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-112">[Get site by path][]</span></span>     | <span data-ttu-id="fd7e4-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="fd7e4-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="fd7e4-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-114">[Get site for a group][]</span></span> | <span data-ttu-id="fd7e4-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="fd7e4-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="fd7e4-116">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-116">[Search for sites][]</span></span>     | <span data-ttu-id="fd7e4-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="fd7e4-117">GET /sites?search={query}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="fd7e4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fd7e4-123">JSON representation</span></span>

<span data-ttu-id="fd7e4-124">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="fd7e4-125">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd7e4-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fd7e4-126">Properties</span></span>

| <span data-ttu-id="fd7e4-127">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="fd7e4-127">Property name</span></span>            | <span data-ttu-id="fd7e4-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd7e4-128">Type</span></span>                                | <span data-ttu-id="fd7e4-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd7e4-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="fd7e4-130">**id**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-130">**id**</span></span>                   | <span data-ttu-id="fd7e4-131">string</span><span class="sxs-lookup"><span data-stu-id="fd7e4-131">string</span></span>                              | <span data-ttu-id="fd7e4-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="fd7e4-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-134">**createdDateTime**</span></span>      | <span data-ttu-id="fd7e4-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd7e4-135">DateTimeOffset</span></span>                      | <span data-ttu-id="fd7e4-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="fd7e4-138">**description**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-138">**description**</span></span>          | <span data-ttu-id="fd7e4-139">string</span><span class="sxs-lookup"><span data-stu-id="fd7e4-139">string</span></span>                              | <span data-ttu-id="fd7e4-140">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="fd7e4-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-141">**displayName**</span></span>          | <span data-ttu-id="fd7e4-142">string</span><span class="sxs-lookup"><span data-stu-id="fd7e4-142">string</span></span>                              | <span data-ttu-id="fd7e4-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="fd7e4-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-145">**eTag**</span></span>                 | <span data-ttu-id="fd7e4-146">string</span><span class="sxs-lookup"><span data-stu-id="fd7e4-146">string</span></span>                              | <span data-ttu-id="fd7e4-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="fd7e4-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="fd7e4-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd7e4-150">DateTimeOffset</span></span>                      | <span data-ttu-id="fd7e4-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="fd7e4-153">**name**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-153">**name**</span></span>                 | <span data-ttu-id="fd7e4-154">string</span><span class="sxs-lookup"><span data-stu-id="fd7e4-154">string</span></span>                              | <span data-ttu-id="fd7e4-155">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="fd7e4-156">**root**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-156">**root**</span></span>                 | [<span data-ttu-id="fd7e4-157">root</span><span class="sxs-lookup"><span data-stu-id="fd7e4-157">root</span></span>](root.md)                     | <span data-ttu-id="fd7e4-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="fd7e4-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-160">**sharepointIds**</span></span>        | [<span data-ttu-id="fd7e4-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="fd7e4-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="fd7e4-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="fd7e4-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-164">**siteCollection**</span></span>       | [<span data-ttu-id="fd7e4-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="fd7e4-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="fd7e4-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="fd7e4-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-169">**webUrl**</span></span>               | <span data-ttu-id="fd7e4-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="fd7e4-170">string (url)</span></span>                        | <span data-ttu-id="fd7e4-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="fd7e4-173">Relações</span><span class="sxs-lookup"><span data-stu-id="fd7e4-173">Relationships</span></span>

| <span data-ttu-id="fd7e4-174">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="fd7e4-174">Relationship name</span></span> | <span data-ttu-id="fd7e4-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd7e4-175">Type</span></span>                             | <span data-ttu-id="fd7e4-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd7e4-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="fd7e4-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-177">**columns**</span></span>       | <span data-ttu-id="fd7e4-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="fd7e4-179">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="fd7e4-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-180">**contentTypes**</span></span>  | <span data-ttu-id="fd7e4-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-181">Collection([contentType][])</span></span>      | <span data-ttu-id="fd7e4-182">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="fd7e4-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-183">**drive**</span></span>         | <span data-ttu-id="fd7e4-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-184">[drive][]</span></span>                        | <span data-ttu-id="fd7e4-185">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="fd7e4-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-186">**drives**</span></span>        | <span data-ttu-id="fd7e4-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-187">Collection([drive][])</span></span>            | <span data-ttu-id="fd7e4-188">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="fd7e4-189">**items**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-189">**items**</span></span>         | <span data-ttu-id="fd7e4-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="fd7e4-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="fd7e4-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-193">**lists**</span></span>         | <span data-ttu-id="fd7e4-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-194">Collection([list][])</span></span>             | <span data-ttu-id="fd7e4-195">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="fd7e4-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-196">**sites**</span></span>         | <span data-ttu-id="fd7e4-197">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="fd7e4-197">Collection([site][])</span></span>             | <span data-ttu-id="fd7e4-198">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="fd7e4-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="fd7e4-199">**onenote**</span></span>       | <span data-ttu-id="fd7e4-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="fd7e4-200">[onenote][]</span></span>                      | <span data-ttu-id="fd7e4-201">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="fd7e4-201">Calls the OneNote service for notebook related operations.</span></span>

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
