---
author: rahmit
description: Esse recurso representa uma página na lista SitePages.
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240ab50f31d500fad960768bb6c45cb9c6ff6511
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965044"
---
# <a name="sitepage-resource"></a><span data-ttu-id="da1e3-103">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="da1e3-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da1e3-104">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="da1e3-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="da1e3-105">Ele contém o título, o layout e uma coleção de [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="da1e3-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="da1e3-106">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="da1e3-106">Tasks on a page</span></span>

<span data-ttu-id="da1e3-107">As tarefas a seguir estão disponíveis para recursos do **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="da1e3-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="da1e3-108">Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.</span><span class="sxs-lookup"><span data-stu-id="da1e3-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="da1e3-109">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="da1e3-109">Common task</span></span>                     | <span data-ttu-id="da1e3-110">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="da1e3-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="da1e3-111">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-111">[List pages][]</span></span>                  | <span data-ttu-id="da1e3-112">OBTER/Pages</span><span class="sxs-lookup"><span data-stu-id="da1e3-112">GET /pages</span></span>
| <span data-ttu-id="da1e3-113">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-113">[Get page][]</span></span>                    | <span data-ttu-id="da1e3-114">OBTER/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="da1e3-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="da1e3-115">[Create][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-115">[Create][]</span></span>                      | <span data-ttu-id="da1e3-116">POSTAR/Pages</span><span class="sxs-lookup"><span data-stu-id="da1e3-116">POST /pages</span></span>
| <span data-ttu-id="da1e3-117">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-117">[Delete][]</span></span>                      | <span data-ttu-id="da1e3-118">EXCLUIR/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="da1e3-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="da1e3-119">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-119">[Publish][]</span></span>                     | <span data-ttu-id="da1e3-120">POSTAR/Pages/{Page-ID}/Publish</span><span class="sxs-lookup"><span data-stu-id="da1e3-120">POST /pages/{page-id}/publish</span></span>

[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="da1e3-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da1e3-126">JSON representation</span></span>

<span data-ttu-id="da1e3-127">Veja a seguir uma representação JSON de um recurso **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="da1e3-127">Here is a JSON representation of a **sitePage** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.sitePage",
  "openType": true
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },

  /* page content */
  "title": "string",
  "pageLayoutType": "String",
  "webParts": [{ "@odata.type": "microsoft.graph.webPart" }],

  /* authoring metadata */
  "publishingState": { "@odata.type": "microsoft.graph.publicationFacet" },

   /* inherited from baseItem */
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="da1e3-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da1e3-128">Properties</span></span>

<span data-ttu-id="da1e3-129">O recurso **sitePage** tem as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="da1e3-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="da1e3-130">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da1e3-130">Property name</span></span>    | <span data-ttu-id="da1e3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="da1e3-131">Type</span></span>                         | <span data-ttu-id="da1e3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="da1e3-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="da1e3-133">contentType</span><span class="sxs-lookup"><span data-stu-id="da1e3-133">contentType</span></span>      | <span data-ttu-id="da1e3-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="da1e3-135">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="da1e3-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="da1e3-136">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="da1e3-136">Page Content</span></span>

<span data-ttu-id="da1e3-137">O recurso **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="da1e3-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="da1e3-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da1e3-138">Property name</span></span>      | <span data-ttu-id="da1e3-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="da1e3-139">Type</span></span>                       | <span data-ttu-id="da1e3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="da1e3-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="da1e3-141">title</span><span class="sxs-lookup"><span data-stu-id="da1e3-141">title</span></span>              | <span data-ttu-id="da1e3-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da1e3-142">string</span></span>                     | <span data-ttu-id="da1e3-143">O título da página.</span><span class="sxs-lookup"><span data-stu-id="da1e3-143">The title of the page.</span></span>
| <span data-ttu-id="da1e3-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="da1e3-144">pageLayout</span></span>         | <span data-ttu-id="da1e3-145">string</span><span class="sxs-lookup"><span data-stu-id="da1e3-145">string</span></span>                     | <span data-ttu-id="da1e3-146">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="da1e3-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="da1e3-147">webParts</span><span class="sxs-lookup"><span data-stu-id="da1e3-147">webParts</span></span>           | <span data-ttu-id="da1e3-148">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-148">[webPart][]</span></span>                | <span data-ttu-id="da1e3-149">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="da1e3-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="da1e3-150">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="da1e3-150">Authoring Metadata</span></span>

<span data-ttu-id="da1e3-151">O recurso **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="da1e3-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="da1e3-152">A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.</span><span class="sxs-lookup"><span data-stu-id="da1e3-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="da1e3-153">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da1e3-153">Property name</span></span>          | <span data-ttu-id="da1e3-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="da1e3-154">Type</span></span>                   | <span data-ttu-id="da1e3-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="da1e3-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="da1e3-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="da1e3-156">publishingState</span></span>        | <span data-ttu-id="da1e3-157">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-157">[publicationFacet][]</span></span>   | <span data-ttu-id="da1e3-158">O status de publicação e a versão do MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="da1e3-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="da1e3-159">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="da1e3-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="da1e3-160">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da1e3-160">Property name</span></span>        | <span data-ttu-id="da1e3-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="da1e3-161">Type</span></span>              | <span data-ttu-id="da1e3-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="da1e3-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="da1e3-163">id</span><span class="sxs-lookup"><span data-stu-id="da1e3-163">id</span></span>                   | <span data-ttu-id="da1e3-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="da1e3-164">string</span></span>            | <span data-ttu-id="da1e3-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="da1e3-167">name</span><span class="sxs-lookup"><span data-stu-id="da1e3-167">name</span></span>                 | <span data-ttu-id="da1e3-168">string</span><span class="sxs-lookup"><span data-stu-id="da1e3-168">string</span></span>            | <span data-ttu-id="da1e3-169">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="da1e3-169">The name / title of the item.</span></span>
| <span data-ttu-id="da1e3-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="da1e3-170">createdBy</span></span>            | <span data-ttu-id="da1e3-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-171">[identitySet][]</span></span>   | <span data-ttu-id="da1e3-172">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="da1e3-172">Identity of the creator of this item.</span></span> <span data-ttu-id="da1e3-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-173">Read-only.</span></span>
| <span data-ttu-id="da1e3-174">eTag</span><span class="sxs-lookup"><span data-stu-id="da1e3-174">eTag</span></span>                 | <span data-ttu-id="da1e3-175">string</span><span class="sxs-lookup"><span data-stu-id="da1e3-175">string</span></span>            | <span data-ttu-id="da1e3-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="da1e3-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="da1e3-178">lastModifiedBy</span></span>       | <span data-ttu-id="da1e3-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-179">[identitySet][]</span></span>   | <span data-ttu-id="da1e3-180">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="da1e3-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="da1e3-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-181">Read-only.</span></span>
| <span data-ttu-id="da1e3-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da1e3-182">lastModifiedDateTime</span></span> | <span data-ttu-id="da1e3-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da1e3-183">DateTimeOffset</span></span>    | <span data-ttu-id="da1e3-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="da1e3-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="da1e3-186">parentReference</span></span>      | <span data-ttu-id="da1e3-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="da1e3-187">[itemReference][]</span></span> | <span data-ttu-id="da1e3-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="da1e3-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="da1e3-190">webUrl</span></span>               | <span data-ttu-id="da1e3-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="da1e3-191">string (url)</span></span>      | <span data-ttu-id="da1e3-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da1e3-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="da1e3-194">Relações</span><span class="sxs-lookup"><span data-stu-id="da1e3-194">Relationships</span></span>

<span data-ttu-id="da1e3-195">O recurso **sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="da1e3-195">The **sitePage** resource does not have relationships to other resources.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[list]: list.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[publicationFacet]: publicationfacet.md
[site]: site.md
[webPart]: webpart.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Page",
  "tocBookmarks": {
    "Page": "#"
  },
  "suppressions": []
}
-->

<!--
TODO:
* Define {page-id}
* Update examples
    * Be consistent with other URLs in the documentation.
    * Try to use the same site, library, etc.
    * Add the URL to the underlying list item resource in the API
* PATCH for list item patches /item/{item-id}/fields.
-->
