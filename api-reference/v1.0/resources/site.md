---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d4dfb3f340a2b2b7ff5ad5a3c9279cb2a03c63be
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482088"
---
# <a name="site-resource"></a><span data-ttu-id="54e5b-102">Recurso site</span><span class="sxs-lookup"><span data-stu-id="54e5b-102">Site resource</span></span>

<span data-ttu-id="54e5b-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="54e5b-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="54e5b-104">Tarefas</span><span class="sxs-lookup"><span data-stu-id="54e5b-104">Tasks</span></span>

<span data-ttu-id="54e5b-105">Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="54e5b-105">All examples below are relative to a list, eg: `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="54e5b-106">Nome da tarefa</span><span class="sxs-lookup"><span data-stu-id="54e5b-106">Task name</span></span>                | <span data-ttu-id="54e5b-107">Exemplo de Solicitação</span><span class="sxs-lookup"><span data-stu-id="54e5b-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="54e5b-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-108">[Get root site][]</span></span>        | <span data-ttu-id="54e5b-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="54e5b-109">GET /sites/root</span></span>
| <span data-ttu-id="54e5b-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-110">[Get site][]</span></span>             | <span data-ttu-id="54e5b-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="54e5b-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="54e5b-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-112">[Get site by path][]</span></span>     | <span data-ttu-id="54e5b-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="54e5b-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="54e5b-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-114">[Get site for a group][]</span></span> | <span data-ttu-id="54e5b-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="54e5b-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="54e5b-116">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-116">[Search for sites][]</span></span>     | <span data-ttu-id="54e5b-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="54e5b-117">GET /sites?search={query}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="54e5b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54e5b-123">JSON representation</span></span>

<span data-ttu-id="54e5b-124">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="54e5b-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="54e5b-125">O recurso **site** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="54e5b-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="54e5b-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54e5b-126">Properties</span></span>

| <span data-ttu-id="54e5b-127">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="54e5b-127">Property name</span></span>            | <span data-ttu-id="54e5b-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="54e5b-128">Type</span></span>                                | <span data-ttu-id="54e5b-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e5b-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="54e5b-130">**id**</span><span class="sxs-lookup"><span data-stu-id="54e5b-130">**id**</span></span>                   | <span data-ttu-id="54e5b-131">string</span><span class="sxs-lookup"><span data-stu-id="54e5b-131">string</span></span>                              | <span data-ttu-id="54e5b-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="54e5b-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="54e5b-134">**createdDateTime**</span></span>      | <span data-ttu-id="54e5b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e5b-135">DateTimeOffset</span></span>                      | <span data-ttu-id="54e5b-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="54e5b-138">**description**</span><span class="sxs-lookup"><span data-stu-id="54e5b-138">**description**</span></span>          | <span data-ttu-id="54e5b-139">string</span><span class="sxs-lookup"><span data-stu-id="54e5b-139">string</span></span>                              | <span data-ttu-id="54e5b-140">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="54e5b-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="54e5b-141">**displayName**</span></span>          | <span data-ttu-id="54e5b-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54e5b-142">string</span></span>                              | <span data-ttu-id="54e5b-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="54e5b-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="54e5b-145">**eTag**</span></span>                 | <span data-ttu-id="54e5b-146">string</span><span class="sxs-lookup"><span data-stu-id="54e5b-146">string</span></span>                              | <span data-ttu-id="54e5b-p104">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="54e5b-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="54e5b-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="54e5b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e5b-150">DateTimeOffset</span></span>                      | <span data-ttu-id="54e5b-p105">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="54e5b-153">**name**</span><span class="sxs-lookup"><span data-stu-id="54e5b-153">**name**</span></span>                 | <span data-ttu-id="54e5b-154">string</span><span class="sxs-lookup"><span data-stu-id="54e5b-154">string</span></span>                              | <span data-ttu-id="54e5b-155">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="54e5b-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="54e5b-156">**root**</span><span class="sxs-lookup"><span data-stu-id="54e5b-156">**root**</span></span>                 | [<span data-ttu-id="54e5b-157">root</span><span class="sxs-lookup"><span data-stu-id="54e5b-157">root</span></span>](root.md)                     | <span data-ttu-id="54e5b-p106">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="54e5b-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="54e5b-160">**sharepointIds**</span></span>        | [<span data-ttu-id="54e5b-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="54e5b-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="54e5b-p107">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="54e5b-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="54e5b-164">**siteCollection**</span></span>       | [<span data-ttu-id="54e5b-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="54e5b-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="54e5b-p108">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="54e5b-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="54e5b-169">**webUrl**</span></span>               | <span data-ttu-id="54e5b-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="54e5b-170">string (url)</span></span>                        | <span data-ttu-id="54e5b-p109">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="54e5b-173">Relações</span><span class="sxs-lookup"><span data-stu-id="54e5b-173">Relationships</span></span>

| <span data-ttu-id="54e5b-174">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="54e5b-174">Relationship name</span></span> | <span data-ttu-id="54e5b-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="54e5b-175">Type</span></span>                             | <span data-ttu-id="54e5b-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e5b-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="54e5b-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="54e5b-177">**columns**</span></span>       | <span data-ttu-id="54e5b-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="54e5b-179">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="54e5b-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="54e5b-180">**contentTypes**</span></span>  | <span data-ttu-id="54e5b-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-181">Collection([contentType][])</span></span>      | <span data-ttu-id="54e5b-182">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="54e5b-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="54e5b-183">**drive**</span></span>         | <span data-ttu-id="54e5b-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-184">[drive][]</span></span>                        | <span data-ttu-id="54e5b-185">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="54e5b-186">**drives**</span><span class="sxs-lookup"><span data-stu-id="54e5b-186">**drives**</span></span>        | <span data-ttu-id="54e5b-187">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-187">Collection([drive][])</span></span>            | <span data-ttu-id="54e5b-188">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="54e5b-189">**items**</span><span class="sxs-lookup"><span data-stu-id="54e5b-189">**items**</span></span>         | <span data-ttu-id="54e5b-190">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="54e5b-p110">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="54e5b-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="54e5b-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="54e5b-193">**lists**</span></span>         | <span data-ttu-id="54e5b-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-194">Collection([list][])</span></span>             | <span data-ttu-id="54e5b-195">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="54e5b-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="54e5b-196">**sites**</span></span>         | <span data-ttu-id="54e5b-197">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="54e5b-197">Collection([site][])</span></span>             | <span data-ttu-id="54e5b-198">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="54e5b-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="54e5b-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="54e5b-199">**OneNote**</span></span>       | <span data-ttu-id="54e5b-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="54e5b-200">[OneNote][]</span></span>                      | <span data-ttu-id="54e5b-201">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="54e5b-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md
[OneNote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
