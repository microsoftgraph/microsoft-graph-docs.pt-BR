---
author: rahmit
description: Esse recurso representa uma página na lista SitePages.
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5562c0e60f0e36acf3621a160c1801d49661ea5c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440112"
---
# <a name="sitepage-resource"></a><span data-ttu-id="bdf8c-103">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="bdf8c-103">sitePage resource</span></span>

<span data-ttu-id="bdf8c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf8c-105">Esse recurso representa uma página [][]na lista SitePages.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-105">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="bdf8c-106">Ele contém o título, o layout e uma coleção de [webParts.][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-106">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="bdf8c-107">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="bdf8c-107">Tasks on a page</span></span>

<span data-ttu-id="bdf8c-108">As tarefas a seguir estão disponíveis para recursos **sitePage.**</span><span class="sxs-lookup"><span data-stu-id="bdf8c-108">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="bdf8c-109">Todos os exemplos são relativos a um [site;][] por exemplo, `https://graph.microsoft.com/{api-version}/sites/{site-id}` .</span><span class="sxs-lookup"><span data-stu-id="bdf8c-109">All examples are relative to a [site][]; for example, `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="bdf8c-110">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="bdf8c-110">Common task</span></span>                     | <span data-ttu-id="bdf8c-111">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf8c-111">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="bdf8c-112">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-112">[List pages][]</span></span>                  | <span data-ttu-id="bdf8c-113">GET /pages</span><span class="sxs-lookup"><span data-stu-id="bdf8c-113">GET /pages</span></span>
| <span data-ttu-id="bdf8c-114">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-114">[Get page][]</span></span>                    | <span data-ttu-id="bdf8c-115">GET /pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="bdf8c-115">GET /pages/{page-id}</span></span>
| <span data-ttu-id="bdf8c-116">[Create][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-116">[Create][]</span></span>                      | <span data-ttu-id="bdf8c-117">POST /pages</span><span class="sxs-lookup"><span data-stu-id="bdf8c-117">POST /pages</span></span>
| <span data-ttu-id="bdf8c-118">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-118">[Delete][]</span></span>                      | <span data-ttu-id="bdf8c-119">DELETE /pages/{page-id}</span><span class="sxs-lookup"><span data-stu-id="bdf8c-119">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="bdf8c-120">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-120">[Publish][]</span></span>                     | <span data-ttu-id="bdf8c-121">POST /pages/{page-id}/publish</span><span class="sxs-lookup"><span data-stu-id="bdf8c-121">POST /pages/{page-id}/publish</span></span>

[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="bdf8c-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdf8c-127">JSON representation</span></span>

<span data-ttu-id="bdf8c-128">Aqui está uma representação JSON de um **recurso sitePage.**</span><span class="sxs-lookup"><span data-stu-id="bdf8c-128">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bdf8c-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdf8c-129">Properties</span></span>

<span data-ttu-id="bdf8c-130">O **recurso sitePage** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-130">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="bdf8c-131">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf8c-131">Property name</span></span>    | <span data-ttu-id="bdf8c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf8c-132">Type</span></span>                         | <span data-ttu-id="bdf8c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8c-133">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="bdf8c-134">contentType</span><span class="sxs-lookup"><span data-stu-id="bdf8c-134">contentType</span></span>      | <span data-ttu-id="bdf8c-135">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-135">[contentTypeInfo][]</span></span>          | <span data-ttu-id="bdf8c-136">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-136">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="bdf8c-137">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="bdf8c-137">Page Content</span></span>

<span data-ttu-id="bdf8c-138">O **recurso sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-138">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="bdf8c-139">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf8c-139">Property name</span></span>      | <span data-ttu-id="bdf8c-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf8c-140">Type</span></span>                       | <span data-ttu-id="bdf8c-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8c-141">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="bdf8c-142">title</span><span class="sxs-lookup"><span data-stu-id="bdf8c-142">title</span></span>              | <span data-ttu-id="bdf8c-143">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdf8c-143">string</span></span>                     | <span data-ttu-id="bdf8c-144">O título da página.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-144">The title of the page.</span></span>
| <span data-ttu-id="bdf8c-145">pageLayout</span><span class="sxs-lookup"><span data-stu-id="bdf8c-145">pageLayout</span></span>         | <span data-ttu-id="bdf8c-146">string</span><span class="sxs-lookup"><span data-stu-id="bdf8c-146">string</span></span>                     | <span data-ttu-id="bdf8c-147">O nome do layout da página.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-147">The name of the page layout of the page.</span></span>
| <span data-ttu-id="bdf8c-148">webParts</span><span class="sxs-lookup"><span data-stu-id="bdf8c-148">webParts</span></span>           | <span data-ttu-id="bdf8c-149">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-149">[webPart][]</span></span>                | <span data-ttu-id="bdf8c-150">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-150">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="bdf8c-151">Autor de metadados</span><span class="sxs-lookup"><span data-stu-id="bdf8c-151">Authoring Metadata</span></span>

<span data-ttu-id="bdf8c-152">O **recurso sitePage** tem os seguintes metadados relacionados à autoria.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-152">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="bdf8c-153">A **propriedade publishingState** refletirá o estado de autoria da página como check-out ou publicado.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-153">The **publishingState** property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="bdf8c-154">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf8c-154">Property name</span></span>          | <span data-ttu-id="bdf8c-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf8c-155">Type</span></span>                   | <span data-ttu-id="bdf8c-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8c-156">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="bdf8c-157">publishingState</span><span class="sxs-lookup"><span data-stu-id="bdf8c-157">publishingState</span></span>        | <span data-ttu-id="bdf8c-158">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-158">[publicationFacet][]</span></span>   | <span data-ttu-id="bdf8c-159">O status de publicação e a MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-159">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="bdf8c-160">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="bdf8c-161">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bdf8c-161">Property name</span></span>        | <span data-ttu-id="bdf8c-162">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdf8c-162">Type</span></span>              | <span data-ttu-id="bdf8c-163">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf8c-163">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="bdf8c-164">id</span><span class="sxs-lookup"><span data-stu-id="bdf8c-164">id</span></span>                   | <span data-ttu-id="bdf8c-165">string</span><span class="sxs-lookup"><span data-stu-id="bdf8c-165">string</span></span>            | <span data-ttu-id="bdf8c-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="bdf8c-168">name</span><span class="sxs-lookup"><span data-stu-id="bdf8c-168">name</span></span>                 | <span data-ttu-id="bdf8c-169">string</span><span class="sxs-lookup"><span data-stu-id="bdf8c-169">string</span></span>            | <span data-ttu-id="bdf8c-170">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-170">The name / title of the item.</span></span>
| <span data-ttu-id="bdf8c-171">createdBy</span><span class="sxs-lookup"><span data-stu-id="bdf8c-171">createdBy</span></span>            | <span data-ttu-id="bdf8c-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-172">[identitySet][]</span></span>   | <span data-ttu-id="bdf8c-173">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-173">Identity of the creator of this item.</span></span> <span data-ttu-id="bdf8c-174">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-174">Read-only.</span></span>
| <span data-ttu-id="bdf8c-175">eTag</span><span class="sxs-lookup"><span data-stu-id="bdf8c-175">eTag</span></span>                 | <span data-ttu-id="bdf8c-176">string</span><span class="sxs-lookup"><span data-stu-id="bdf8c-176">string</span></span>            | <span data-ttu-id="bdf8c-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="bdf8c-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="bdf8c-179">lastModifiedBy</span></span>       | <span data-ttu-id="bdf8c-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-180">[identitySet][]</span></span>   | <span data-ttu-id="bdf8c-181">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="bdf8c-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-182">Read-only.</span></span>
| <span data-ttu-id="bdf8c-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdf8c-183">lastModifiedDateTime</span></span> | <span data-ttu-id="bdf8c-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdf8c-184">DateTimeOffset</span></span>    | <span data-ttu-id="bdf8c-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bdf8c-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="bdf8c-187">parentReference</span></span>      | <span data-ttu-id="bdf8c-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bdf8c-188">[itemReference][]</span></span> | <span data-ttu-id="bdf8c-189">Informações do pai, se o item tiver um pai.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-189">Parent information, if the item has a parent.</span></span> <span data-ttu-id="bdf8c-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-190">Read-only.</span></span>
| <span data-ttu-id="bdf8c-191">webUrl</span><span class="sxs-lookup"><span data-stu-id="bdf8c-191">webUrl</span></span>               | <span data-ttu-id="bdf8c-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="bdf8c-192">string (url)</span></span>      | <span data-ttu-id="bdf8c-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="bdf8c-195">Relações</span><span class="sxs-lookup"><span data-stu-id="bdf8c-195">Relationships</span></span>

<span data-ttu-id="bdf8c-196">O **recurso sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="bdf8c-196">The **sitePage** resource does not have relationships to other resources.</span></span>

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


