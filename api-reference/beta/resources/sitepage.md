---
author: rahmit
description: Esse recurso representa uma página na lista SitePages.
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 6b7ce7bc14ce95ec4573fb7660cb584703d4a54e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520531"
---
# <a name="sitepage-resource"></a><span data-ttu-id="2df1b-103">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="2df1b-103">sitePage resource</span></span>

<span data-ttu-id="2df1b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2df1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2df1b-105">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="2df1b-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="2df1b-106">Ele contém o título, o layout e uma coleção de [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="2df1b-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="2df1b-107">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="2df1b-107">Tasks on a page</span></span>

<span data-ttu-id="2df1b-108">As tarefas a seguir estão disponíveis para recursos do **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="2df1b-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="2df1b-109">Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.</span><span class="sxs-lookup"><span data-stu-id="2df1b-109">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="2df1b-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="2df1b-110">Common task</span></span>                     | <span data-ttu-id="2df1b-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="2df1b-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="2df1b-112">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-112">[List pages][]</span></span>                  | <span data-ttu-id="2df1b-113">OBTER/Pages</span><span class="sxs-lookup"><span data-stu-id="2df1b-113">GET /pages</span></span>
| <span data-ttu-id="2df1b-114">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-114">[Get page][]</span></span>                    | <span data-ttu-id="2df1b-115">OBTER/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="2df1b-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="2df1b-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-116">[Create][]</span></span>                      | <span data-ttu-id="2df1b-117">POSTAR/Pages</span><span class="sxs-lookup"><span data-stu-id="2df1b-117">POST /pages</span></span>
| <span data-ttu-id="2df1b-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-118">[Delete][]</span></span>                      | <span data-ttu-id="2df1b-119">EXCLUIR/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="2df1b-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="2df1b-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-120">[Publish][]</span></span>                     | <span data-ttu-id="2df1b-121">POSTAR/Pages/{Page-ID}/Publish</span><span class="sxs-lookup"><span data-stu-id="2df1b-121">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="2df1b-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2df1b-127">JSON representation</span></span>

<span data-ttu-id="2df1b-128">Veja a seguir uma representação JSON de um recurso **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="2df1b-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2df1b-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2df1b-129">Properties</span></span>

<span data-ttu-id="2df1b-130">O recurso **sitePage** tem as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="2df1b-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="2df1b-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df1b-131">Property name</span></span>    | <span data-ttu-id="2df1b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df1b-132">Type</span></span>                         | <span data-ttu-id="2df1b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df1b-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="2df1b-134">contentType</span><span class="sxs-lookup"><span data-stu-id="2df1b-134">contentType</span></span>      | <span data-ttu-id="2df1b-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="2df1b-136">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="2df1b-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="2df1b-137">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="2df1b-137">Page Content</span></span>

<span data-ttu-id="2df1b-138">O recurso **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2df1b-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="2df1b-139">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df1b-139">Property name</span></span>      | <span data-ttu-id="2df1b-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df1b-140">Type</span></span>                       | <span data-ttu-id="2df1b-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df1b-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="2df1b-142">title</span><span class="sxs-lookup"><span data-stu-id="2df1b-142">title</span></span>              | <span data-ttu-id="2df1b-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df1b-143">string</span></span>                     | <span data-ttu-id="2df1b-144">O título da página.</span><span class="sxs-lookup"><span data-stu-id="2df1b-144">The title of the page.</span></span>
| <span data-ttu-id="2df1b-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="2df1b-145">pageLayout</span></span>         | <span data-ttu-id="2df1b-146">string</span><span class="sxs-lookup"><span data-stu-id="2df1b-146">string</span></span>                     | <span data-ttu-id="2df1b-147">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="2df1b-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="2df1b-148">webParts</span><span class="sxs-lookup"><span data-stu-id="2df1b-148">webParts</span></span>           | <span data-ttu-id="2df1b-149">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-149">[webPart][]</span></span>                | <span data-ttu-id="2df1b-150">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="2df1b-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="2df1b-151">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="2df1b-151">Authoring Metadata</span></span>

<span data-ttu-id="2df1b-152">O recurso **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="2df1b-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="2df1b-153">A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.</span><span class="sxs-lookup"><span data-stu-id="2df1b-153">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="2df1b-154">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df1b-154">Property name</span></span>          | <span data-ttu-id="2df1b-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df1b-155">Type</span></span>                   | <span data-ttu-id="2df1b-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df1b-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="2df1b-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="2df1b-157">publishingState</span></span>        | <span data-ttu-id="2df1b-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-158">[publicationFacet][]</span></span>   | <span data-ttu-id="2df1b-159">O status de publicação e a versão do MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="2df1b-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="2df1b-160">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="2df1b-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="2df1b-161">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="2df1b-161">Property name</span></span>        | <span data-ttu-id="2df1b-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df1b-162">Type</span></span>              | <span data-ttu-id="2df1b-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df1b-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="2df1b-164">id</span><span class="sxs-lookup"><span data-stu-id="2df1b-164">id</span></span>                   | <span data-ttu-id="2df1b-165">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df1b-165">string</span></span>            | <span data-ttu-id="2df1b-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="2df1b-168">name</span><span class="sxs-lookup"><span data-stu-id="2df1b-168">name</span></span>                 | <span data-ttu-id="2df1b-169">string</span><span class="sxs-lookup"><span data-stu-id="2df1b-169">string</span></span>            | <span data-ttu-id="2df1b-170">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="2df1b-170">The name / title of the item.</span></span>
| <span data-ttu-id="2df1b-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="2df1b-171">createdBy</span></span>            | <span data-ttu-id="2df1b-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-172">[identitySet][]</span></span>   | <span data-ttu-id="2df1b-173">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="2df1b-173">Identity of the creator of this item.</span></span> <span data-ttu-id="2df1b-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-174">Read-only.</span></span>
| <span data-ttu-id="2df1b-175">eTag</span><span class="sxs-lookup"><span data-stu-id="2df1b-175">eTag</span></span>                 | <span data-ttu-id="2df1b-176">string</span><span class="sxs-lookup"><span data-stu-id="2df1b-176">string</span></span>            | <span data-ttu-id="2df1b-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="2df1b-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2df1b-179">lastModifiedBy</span></span>       | <span data-ttu-id="2df1b-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-180">[identitySet][]</span></span>   | <span data-ttu-id="2df1b-181">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="2df1b-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="2df1b-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-182">Read-only.</span></span>
| <span data-ttu-id="2df1b-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2df1b-183">lastModifiedDateTime</span></span> | <span data-ttu-id="2df1b-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2df1b-184">DateTimeOffset</span></span>    | <span data-ttu-id="2df1b-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="2df1b-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="2df1b-187">parentReference</span></span>      | <span data-ttu-id="2df1b-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2df1b-188">[itemReference][]</span></span> | <span data-ttu-id="2df1b-189">Informações do pai, se o item tiver um pai.</span><span class="sxs-lookup"><span data-stu-id="2df1b-189">Parent information, if the item has a parent.</span></span> <span data-ttu-id="2df1b-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-190">Read-only.</span></span>
| <span data-ttu-id="2df1b-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="2df1b-191">webUrl</span></span>               | <span data-ttu-id="2df1b-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="2df1b-192">string (url)</span></span>      | <span data-ttu-id="2df1b-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2df1b-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="2df1b-195">Relações</span><span class="sxs-lookup"><span data-stu-id="2df1b-195">Relationships</span></span>

<span data-ttu-id="2df1b-196">O recurso **sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="2df1b-196">The **sitePage** resource does not have relationships to other resources.</span></span>

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
