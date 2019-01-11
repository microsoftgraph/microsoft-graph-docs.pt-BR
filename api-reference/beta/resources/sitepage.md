---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.openlocfilehash: d4673138106e23afedb5ff0f28d8ce72fa2797b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871488"
---
# <a name="sitepage-resource"></a><span data-ttu-id="504af-102">recurso de sitePage</span><span class="sxs-lookup"><span data-stu-id="504af-102">sitePage resource</span></span>

> <span data-ttu-id="504af-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="504af-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="504af-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="504af-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="504af-105">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="504af-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="504af-106">Ele contém uma coleção de [Web Part][]s, layout e o título.</span><span class="sxs-lookup"><span data-stu-id="504af-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="504af-107">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="504af-107">Tasks on a page</span></span>

<span data-ttu-id="504af-108">As tarefas a seguir estão disponíveis para os recursos de **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="504af-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="504af-109">Todos os exemplos a seguir são em relação um [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="504af-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="504af-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="504af-110">Common task</span></span>                     | <span data-ttu-id="504af-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="504af-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="504af-112">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="504af-112">[List pages][]</span></span>                  | <span data-ttu-id="504af-113">OBTER /pages</span><span class="sxs-lookup"><span data-stu-id="504af-113">GET /pages</span></span>
| <span data-ttu-id="504af-114">[Get page][]</span><span class="sxs-lookup"><span data-stu-id="504af-114">[Get page][]</span></span>                    | <span data-ttu-id="504af-115">OBTER /pages/ {id page}</span><span class="sxs-lookup"><span data-stu-id="504af-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="504af-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="504af-116">[Create][]</span></span>                      | <span data-ttu-id="504af-117">/Pages POST</span><span class="sxs-lookup"><span data-stu-id="504af-117">POST /pages</span></span>
| <span data-ttu-id="504af-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="504af-118">[Delete][]</span></span>                      | <span data-ttu-id="504af-119">Excluir /pages/ {id page}</span><span class="sxs-lookup"><span data-stu-id="504af-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="504af-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="504af-120">[Publish][]</span></span>                     | <span data-ttu-id="504af-121">POSTAR /pages/ {id page} / publicar</span><span class="sxs-lookup"><span data-stu-id="504af-121">POST /pages/{page-id}/publish</span></span>

[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="504af-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="504af-127">JSON representation</span></span>

<span data-ttu-id="504af-128">Aqui está uma representação JSON de um recurso de **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="504af-128">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayout": "Article",
  "webParts": [{ "@odata.type": "microsoft.graph.sitePageWebParts" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

  /* inherited from baseItem */
  "id": "string",
  "name": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="504af-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="504af-129">Properties</span></span>

<span data-ttu-id="504af-130">O recurso de **sitePage** possui as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="504af-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="504af-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="504af-131">Property name</span></span>    | <span data-ttu-id="504af-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="504af-132">Type</span></span>                         | <span data-ttu-id="504af-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="504af-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="504af-134">contentType</span><span class="sxs-lookup"><span data-stu-id="504af-134">contentType</span></span>      | <span data-ttu-id="504af-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="504af-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="504af-136">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="504af-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="504af-137">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="504af-137">Page Content</span></span>

<span data-ttu-id="504af-138">O recurso de **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="504af-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="504af-139">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="504af-139">Property name</span></span>      | <span data-ttu-id="504af-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="504af-140">Type</span></span>                       | <span data-ttu-id="504af-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="504af-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="504af-142">title</span><span class="sxs-lookup"><span data-stu-id="504af-142">title</span></span>              | <span data-ttu-id="504af-143">string</span><span class="sxs-lookup"><span data-stu-id="504af-143">string</span></span>                     | <span data-ttu-id="504af-144">O título da página.</span><span class="sxs-lookup"><span data-stu-id="504af-144">The title of the page.</span></span>
| <span data-ttu-id="504af-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="504af-145">pageLayout</span></span>         | <span data-ttu-id="504af-146">string</span><span class="sxs-lookup"><span data-stu-id="504af-146">string</span></span>                     | <span data-ttu-id="504af-147">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="504af-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="504af-148">Web Parts</span><span class="sxs-lookup"><span data-stu-id="504af-148">webParts</span></span>           | <span data-ttu-id="504af-149">[Web Part][]</span><span class="sxs-lookup"><span data-stu-id="504af-149">[webPart][]</span></span>                | <span data-ttu-id="504af-150">As web parts na página.</span><span class="sxs-lookup"><span data-stu-id="504af-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="504af-151">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="504af-151">Authoring Metadata</span></span>

<span data-ttu-id="504af-152">O recurso de **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="504af-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="504af-153">A propriedade publishingState irão refletir a estado como check-out ou publicada de criação de páginas.</span><span class="sxs-lookup"><span data-stu-id="504af-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="504af-154">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="504af-154">Property name</span></span>          | <span data-ttu-id="504af-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="504af-155">Type</span></span>                   | <span data-ttu-id="504af-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="504af-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="504af-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="504af-157">publishingState</span></span>        | <span data-ttu-id="504af-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="504af-158">[publicationFacet][]</span></span>   | <span data-ttu-id="504af-159">O status de publicação e a versão de MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="504af-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="504af-160">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="504af-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="504af-161">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="504af-161">Property name</span></span>        | <span data-ttu-id="504af-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="504af-162">Type</span></span>              | <span data-ttu-id="504af-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="504af-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="504af-164">id</span><span class="sxs-lookup"><span data-stu-id="504af-164">id</span></span>                   | <span data-ttu-id="504af-165">string</span><span class="sxs-lookup"><span data-stu-id="504af-165">string</span></span>            | <span data-ttu-id="504af-p105">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="504af-168">name</span><span class="sxs-lookup"><span data-stu-id="504af-168">name</span></span>                 | <span data-ttu-id="504af-169">string</span><span class="sxs-lookup"><span data-stu-id="504af-169">string</span></span>            | <span data-ttu-id="504af-170">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="504af-170">The name / title of the item.</span></span>
| <span data-ttu-id="504af-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="504af-171">createdBy</span></span>            | <span data-ttu-id="504af-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="504af-172">[identitySet][]</span></span>   | <span data-ttu-id="504af-173">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="504af-173">Identity of the creator of this item.</span></span> <span data-ttu-id="504af-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-174">Read-only.</span></span>
| <span data-ttu-id="504af-175">eTag</span><span class="sxs-lookup"><span data-stu-id="504af-175">eTag</span></span>                 | <span data-ttu-id="504af-176">string</span><span class="sxs-lookup"><span data-stu-id="504af-176">string</span></span>            | <span data-ttu-id="504af-p107">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-p107">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="504af-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="504af-179">lastModifiedBy</span></span>       | <span data-ttu-id="504af-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="504af-180">[identitySet][]</span></span>   | <span data-ttu-id="504af-181">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="504af-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="504af-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-182">Read-only.</span></span>
| <span data-ttu-id="504af-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="504af-183">lastModifiedDateTime</span></span> | <span data-ttu-id="504af-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504af-184">DateTimeOffset</span></span>    | <span data-ttu-id="504af-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="504af-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="504af-187">parentReference</span></span>      | <span data-ttu-id="504af-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="504af-188">[itemReference][]</span></span> | <span data-ttu-id="504af-p110">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-p110">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="504af-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="504af-191">webUrl</span></span>               | <span data-ttu-id="504af-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="504af-192">string (url)</span></span>      | <span data-ttu-id="504af-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="504af-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="504af-195">Relações</span><span class="sxs-lookup"><span data-stu-id="504af-195">Relationships</span></span>

<span data-ttu-id="504af-196">O recurso de **sitePage** não tem relações para outros recursos.</span><span class="sxs-lookup"><span data-stu-id="504af-196">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[lista]: list.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[Web Part]: webpart.md
[webPart]: webpart.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  }
} -->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
