---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a><span data-ttu-id="dac4c-102">Recurso site</span><span class="sxs-lookup"><span data-stu-id="dac4c-102">Site resource</span></span>

<span data-ttu-id="dac4c-103">O recurso **site** fornece metadados e relações para um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="dac4c-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="dac4c-104">Tarefas</span><span class="sxs-lookup"><span data-stu-id="dac4c-104">Tasks</span></span>

<span data-ttu-id="dac4c-105">Todos os exemplos a seguir referem-se ao endereço `https://graph.microsoft.com/v1.0`.</span><span class="sxs-lookup"><span data-stu-id="dac4c-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="dac4c-106">Nome da tarefa</span><span class="sxs-lookup"><span data-stu-id="dac4c-106">Task name</span></span>                | <span data-ttu-id="dac4c-107">Exemplo de Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac4c-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="dac4c-108">[Obter site raiz][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-108">[Get root site][]</span></span>        | <span data-ttu-id="dac4c-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="dac4c-109">GET /sites/root</span></span>
| <span data-ttu-id="dac4c-110">[Obter site][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-110">[Get site][]</span></span>             | <span data-ttu-id="dac4c-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="dac4c-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="dac4c-112">[Obter site por caminho][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-112">[Get site by path][]</span></span>     | <span data-ttu-id="dac4c-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="dac4c-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="dac4c-114">[Obter o site para um grupo][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-114">[Get site for a group][]</span></span> | <span data-ttu-id="dac4c-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="dac4c-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="dac4c-116">[Procurar sites][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-116">[Search for sites][]</span></span>     | <span data-ttu-id="dac4c-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="dac4c-117">GET /sites?search={query}</span></span>

[Obter site]: ../api/site_get.md
[Obter site raiz]: ../api/site_get.md
[Obter site por caminho]: ../api/site_getbypath.md
[Obter o site para um grupo]: ../api/site_get.md
[Procurar sites]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="dac4c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dac4c-123">JSON representation</span></span>

<span data-ttu-id="dac4c-124">Veja a seguir uma representação JSON de um recurso **site**.</span><span class="sxs-lookup"><span data-stu-id="dac4c-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="dac4c-125">O recurso **driveItem** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="dac4c-125">The **driveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

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
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="dac4c-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dac4c-126">Properties</span></span>

| <span data-ttu-id="dac4c-127">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dac4c-127">Property name</span></span>            | <span data-ttu-id="dac4c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="dac4c-128">Type</span></span>                                | <span data-ttu-id="dac4c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac4c-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="dac4c-130">**id**</span><span class="sxs-lookup"><span data-stu-id="dac4c-130">**id**</span></span>                   | <span data-ttu-id="dac4c-131">string</span><span class="sxs-lookup"><span data-stu-id="dac4c-131">string</span></span>                              | <span data-ttu-id="dac4c-p101">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="dac4c-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="dac4c-134">**createdDateTime**</span></span>      | <span data-ttu-id="dac4c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dac4c-135">DateTimeOffset</span></span>                      | <span data-ttu-id="dac4c-p102">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="dac4c-138">**description**</span><span class="sxs-lookup"><span data-stu-id="dac4c-138">**description**</span></span>          | <span data-ttu-id="dac4c-139">string</span><span class="sxs-lookup"><span data-stu-id="dac4c-139">string</span></span>                              | <span data-ttu-id="dac4c-140">O texto descritivo do site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="dac4c-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="dac4c-141">**displayName**</span></span>          | <span data-ttu-id="dac4c-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dac4c-142">string</span></span>                              | <span data-ttu-id="dac4c-p103">O texto completo do site. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="dac4c-145">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="dac4c-145">**lastModifiedDateTime**</span></span> | <span data-ttu-id="dac4c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dac4c-146">DateTimeOffset</span></span>                      | <span data-ttu-id="dac4c-p104">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p104">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="dac4c-149">**name**</span><span class="sxs-lookup"><span data-stu-id="dac4c-149">**name**</span></span>                 | <span data-ttu-id="dac4c-150">string</span><span class="sxs-lookup"><span data-stu-id="dac4c-150">string</span></span>                              | <span data-ttu-id="dac4c-151">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="dac4c-151">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="dac4c-152">**root**</span><span class="sxs-lookup"><span data-stu-id="dac4c-152">**root**</span></span>                 | [<span data-ttu-id="dac4c-153">root</span><span class="sxs-lookup"><span data-stu-id="dac4c-153">root</span></span>](root.md)                     | <span data-ttu-id="dac4c-p105">Se estiver presente, indica que este é o site raiz do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p105">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="dac4c-156">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="dac4c-156">**sharepointIds**</span></span>        | [<span data-ttu-id="dac4c-157">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="dac4c-157">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="dac4c-p106">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="dac4c-160">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="dac4c-160">**siteCollection**</span></span>       | [<span data-ttu-id="dac4c-161">siteCollection</span><span class="sxs-lookup"><span data-stu-id="dac4c-161">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="dac4c-p107">Fornece detalhes sobre o conjunto de sites do site. Disponível apenas no site raiz. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p107">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="dac4c-165">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="dac4c-165">**webUrl**</span></span>               | <span data-ttu-id="dac4c-166">string (url)</span><span class="sxs-lookup"><span data-stu-id="dac4c-166">string (url)</span></span>                        | <span data-ttu-id="dac4c-p108">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p108">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="dac4c-169">Relações</span><span class="sxs-lookup"><span data-stu-id="dac4c-169">Relationships</span></span>

| <span data-ttu-id="dac4c-170">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="dac4c-170">Relationship name</span></span> | <span data-ttu-id="dac4c-171">Tipo</span><span class="sxs-lookup"><span data-stu-id="dac4c-171">Type</span></span>                             | <span data-ttu-id="dac4c-172">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac4c-172">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="dac4c-173">**columns**</span><span class="sxs-lookup"><span data-stu-id="dac4c-173">**columns**</span></span>       | <span data-ttu-id="dac4c-174">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-174">Collection([columnDefinition][])</span></span> | <span data-ttu-id="dac4c-175">O conjunto de definições de coluna reutilizáveis entre listas nesse site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-175">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="dac4c-176">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="dac4c-176">**contentTypes**</span></span>  | <span data-ttu-id="dac4c-177">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-177">Collection([contentType][])</span></span>      | <span data-ttu-id="dac4c-178">O conjunto de tipos de conteúdo definido para esse site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-178">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="dac4c-179">**drive**</span><span class="sxs-lookup"><span data-stu-id="dac4c-179">**drive**</span></span>         | <span data-ttu-id="dac4c-180">[drive][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-180">[drive][]</span></span>                        | <span data-ttu-id="dac4c-181">A unidade padrão (biblioteca de documentos) desse site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-181">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="dac4c-182">**drives**</span><span class="sxs-lookup"><span data-stu-id="dac4c-182">**drives**</span></span>        | <span data-ttu-id="dac4c-183">Collection([drive][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-183">Collection([drive][])</span></span>            | <span data-ttu-id="dac4c-184">O conjunto de unidades (bibliotecas de documentos) nesse site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-184">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="dac4c-185">**items**</span><span class="sxs-lookup"><span data-stu-id="dac4c-185">**items**</span></span>         | <span data-ttu-id="dac4c-186">Collection([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-186">Collection([baseItem][])</span></span>         | <span data-ttu-id="dac4c-p109">Usado para lidar com qualquer item contido neste site. Não é possível enumerar este conjunto.</span><span class="sxs-lookup"><span data-stu-id="dac4c-p109">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="dac4c-189">**lists**</span><span class="sxs-lookup"><span data-stu-id="dac4c-189">**Lists**</span></span>         | <span data-ttu-id="dac4c-190">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-190">Collection([list][])</span></span>             | <span data-ttu-id="dac4c-191">O conjunto de listas neste site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-191">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="dac4c-192">**sites**</span><span class="sxs-lookup"><span data-stu-id="dac4c-192">**sites**</span></span>         | <span data-ttu-id="dac4c-193">Collection([site][])</span><span class="sxs-lookup"><span data-stu-id="dac4c-193">Collection([site][])</span></span>             | <span data-ttu-id="dac4c-194">O conjunto dos subsites neste site.</span><span class="sxs-lookup"><span data-stu-id="dac4c-194">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="dac4c-195">**onenote**</span><span class="sxs-lookup"><span data-stu-id="dac4c-195">**onenote**</span></span>       | <span data-ttu-id="dac4c-196">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="dac4c-196">[onenote][]</span></span>                      | <span data-ttu-id="dac4c-197">Chama o serviço OneNote para operações relacionadas ao bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="dac4c-197">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
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
