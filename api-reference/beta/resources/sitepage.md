---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640655"
---
# <a name="sitepage-resource"></a><span data-ttu-id="6d29a-102">recurso de sitePage</span><span class="sxs-lookup"><span data-stu-id="6d29a-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d29a-103">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="6d29a-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="6d29a-104">Ele contém uma coleção de [Web Part][]s, layout e o título.</span><span class="sxs-lookup"><span data-stu-id="6d29a-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="6d29a-105">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="6d29a-105">Tasks on a page</span></span>

<span data-ttu-id="6d29a-106">As tarefas a seguir estão disponíveis para os recursos de **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="6d29a-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="6d29a-107">Todos os exemplos a seguir são em relação um [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span><span class="sxs-lookup"><span data-stu-id="6d29a-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="6d29a-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="6d29a-108">Common task</span></span>                     | <span data-ttu-id="6d29a-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="6d29a-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="6d29a-110">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-110">[List pages][]</span></span>                  | <span data-ttu-id="6d29a-111">OBTER /pages</span><span class="sxs-lookup"><span data-stu-id="6d29a-111">GET /pages</span></span>
| <span data-ttu-id="6d29a-112">[Get page][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-112">[Get page][]</span></span>                    | <span data-ttu-id="6d29a-113">OBTER /pages/ {id page}</span><span class="sxs-lookup"><span data-stu-id="6d29a-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="6d29a-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-114">[Create][]</span></span>                      | <span data-ttu-id="6d29a-115">/Pages POST</span><span class="sxs-lookup"><span data-stu-id="6d29a-115">POST /pages</span></span>
| <span data-ttu-id="6d29a-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-116">[Delete][]</span></span>                      | <span data-ttu-id="6d29a-117">Excluir /pages/ {id page}</span><span class="sxs-lookup"><span data-stu-id="6d29a-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="6d29a-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-118">[Publish][]</span></span>                     | <span data-ttu-id="6d29a-119">POSTAR /pages/ {id page} / publicar</span><span class="sxs-lookup"><span data-stu-id="6d29a-119">POST /pages/{page-id}/publish</span></span>

[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="6d29a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d29a-125">JSON representation</span></span>

<span data-ttu-id="6d29a-126">Aqui está uma representação JSON de um recurso de **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="6d29a-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6d29a-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d29a-127">Properties</span></span>

<span data-ttu-id="6d29a-128">O recurso de **sitePage** possui as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="6d29a-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="6d29a-129">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6d29a-129">Property name</span></span>    | <span data-ttu-id="6d29a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d29a-130">Type</span></span>                         | <span data-ttu-id="6d29a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d29a-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="6d29a-132">contentType</span><span class="sxs-lookup"><span data-stu-id="6d29a-132">contentType</span></span>      | <span data-ttu-id="6d29a-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="6d29a-134">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="6d29a-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="6d29a-135">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="6d29a-135">Page Content</span></span>

<span data-ttu-id="6d29a-136">O recurso de **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6d29a-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="6d29a-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6d29a-137">Property name</span></span>      | <span data-ttu-id="6d29a-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d29a-138">Type</span></span>                       | <span data-ttu-id="6d29a-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d29a-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="6d29a-140">title</span><span class="sxs-lookup"><span data-stu-id="6d29a-140">title</span></span>              | <span data-ttu-id="6d29a-141">string</span><span class="sxs-lookup"><span data-stu-id="6d29a-141">string</span></span>                     | <span data-ttu-id="6d29a-142">O título da página.</span><span class="sxs-lookup"><span data-stu-id="6d29a-142">The title of the page.</span></span>
| <span data-ttu-id="6d29a-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="6d29a-143">pageLayout</span></span>         | <span data-ttu-id="6d29a-144">string</span><span class="sxs-lookup"><span data-stu-id="6d29a-144">string</span></span>                     | <span data-ttu-id="6d29a-145">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="6d29a-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="6d29a-146">Web Parts</span><span class="sxs-lookup"><span data-stu-id="6d29a-146">webParts</span></span>           | <span data-ttu-id="6d29a-147">[Web Part][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-147">[webPart][]</span></span>                | <span data-ttu-id="6d29a-148">As web parts na página.</span><span class="sxs-lookup"><span data-stu-id="6d29a-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="6d29a-149">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="6d29a-149">Authoring Metadata</span></span>

<span data-ttu-id="6d29a-150">O recurso de **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="6d29a-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="6d29a-151">A propriedade publishingState irão refletir a estado como check-out ou publicada de criação de páginas.</span><span class="sxs-lookup"><span data-stu-id="6d29a-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="6d29a-152">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6d29a-152">Property name</span></span>          | <span data-ttu-id="6d29a-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d29a-153">Type</span></span>                   | <span data-ttu-id="6d29a-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d29a-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="6d29a-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="6d29a-155">publishingState</span></span>        | <span data-ttu-id="6d29a-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-156">[publicationFacet][]</span></span>   | <span data-ttu-id="6d29a-157">O status de publicação e a versão de MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="6d29a-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="6d29a-158">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="6d29a-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="6d29a-159">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6d29a-159">Property name</span></span>        | <span data-ttu-id="6d29a-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d29a-160">Type</span></span>              | <span data-ttu-id="6d29a-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d29a-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="6d29a-162">id</span><span class="sxs-lookup"><span data-stu-id="6d29a-162">id</span></span>                   | <span data-ttu-id="6d29a-163">string</span><span class="sxs-lookup"><span data-stu-id="6d29a-163">string</span></span>            | <span data-ttu-id="6d29a-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="6d29a-166">name</span><span class="sxs-lookup"><span data-stu-id="6d29a-166">name</span></span>                 | <span data-ttu-id="6d29a-167">string</span><span class="sxs-lookup"><span data-stu-id="6d29a-167">string</span></span>            | <span data-ttu-id="6d29a-168">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="6d29a-168">The name / title of the item.</span></span>
| <span data-ttu-id="6d29a-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="6d29a-169">createdBy</span></span>            | <span data-ttu-id="6d29a-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-170">[identitySet][]</span></span>   | <span data-ttu-id="6d29a-171">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="6d29a-171">Identity of the creator of this item.</span></span> <span data-ttu-id="6d29a-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-172">Read-only.</span></span>
| <span data-ttu-id="6d29a-173">eTag</span><span class="sxs-lookup"><span data-stu-id="6d29a-173">eTag</span></span>                 | <span data-ttu-id="6d29a-174">string</span><span class="sxs-lookup"><span data-stu-id="6d29a-174">string</span></span>            | <span data-ttu-id="6d29a-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="6d29a-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6d29a-177">lastModifiedBy</span></span>       | <span data-ttu-id="6d29a-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-178">[identitySet][]</span></span>   | <span data-ttu-id="6d29a-179">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="6d29a-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="6d29a-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-180">Read-only.</span></span>
| <span data-ttu-id="6d29a-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d29a-181">lastModifiedDateTime</span></span> | <span data-ttu-id="6d29a-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d29a-182">DateTimeOffset</span></span>    | <span data-ttu-id="6d29a-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6d29a-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="6d29a-185">parentReference</span></span>      | <span data-ttu-id="6d29a-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6d29a-186">[itemReference][]</span></span> | <span data-ttu-id="6d29a-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6d29a-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="6d29a-189">webUrl</span></span>               | <span data-ttu-id="6d29a-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="6d29a-190">string (url)</span></span>      | <span data-ttu-id="6d29a-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6d29a-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="6d29a-193">Relações</span><span class="sxs-lookup"><span data-stu-id="6d29a-193">Relationships</span></span>

<span data-ttu-id="6d29a-194">O recurso de **sitePage** não tem relações para outros recursos.</span><span class="sxs-lookup"><span data-stu-id="6d29a-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
[Web Part]: webpart.md
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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitepage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
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
