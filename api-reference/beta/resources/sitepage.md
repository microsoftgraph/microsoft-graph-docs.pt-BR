---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 7b1634e79214f1cece85a78af29db6422ac03a81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583400"
---
# <a name="sitepage-resource"></a><span data-ttu-id="44600-102">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="44600-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44600-103">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="44600-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="44600-104">Ele contém o título, o layout e uma coleção de [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="44600-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="44600-105">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="44600-105">Tasks on a page</span></span>

<span data-ttu-id="44600-106">As tarefas a seguir estão disponíveis para recursos do **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="44600-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="44600-107">Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.</span><span class="sxs-lookup"><span data-stu-id="44600-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="44600-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="44600-108">Common task</span></span>                     | <span data-ttu-id="44600-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="44600-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="44600-110">[Listar páginas][]</span><span class="sxs-lookup"><span data-stu-id="44600-110">[List pages][]</span></span>                  | <span data-ttu-id="44600-111">OBTER/Pages</span><span class="sxs-lookup"><span data-stu-id="44600-111">GET /pages</span></span>
| <span data-ttu-id="44600-112">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="44600-112">[Get page][]</span></span>                    | <span data-ttu-id="44600-113">OBTER/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="44600-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="44600-114">[Create][]</span><span class="sxs-lookup"><span data-stu-id="44600-114">[Create][]</span></span>                      | <span data-ttu-id="44600-115">POSTAR/Pages</span><span class="sxs-lookup"><span data-stu-id="44600-115">POST /pages</span></span>
| <span data-ttu-id="44600-116">[Excluir][]</span><span class="sxs-lookup"><span data-stu-id="44600-116">[Delete][]</span></span>                      | <span data-ttu-id="44600-117">EXCLUIR/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="44600-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="44600-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="44600-118">[Publish][]</span></span>                     | <span data-ttu-id="44600-119">POSTAR/Pages/{Page-ID}/Publish</span><span class="sxs-lookup"><span data-stu-id="44600-119">POST /pages/{page-id}/publish</span></span>

[Listar páginas]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="44600-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44600-125">JSON representation</span></span>

<span data-ttu-id="44600-126">Veja a seguir uma representação JSON de um recurso **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="44600-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="44600-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44600-127">Properties</span></span>

<span data-ttu-id="44600-128">O recurso **sitePage** tem as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="44600-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="44600-129">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44600-129">Property name</span></span>    | <span data-ttu-id="44600-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44600-130">Type</span></span>                         | <span data-ttu-id="44600-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44600-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="44600-132">contentType</span><span class="sxs-lookup"><span data-stu-id="44600-132">contentType</span></span>      | <span data-ttu-id="44600-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="44600-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="44600-134">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="44600-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="44600-135">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="44600-135">Page Content</span></span>

<span data-ttu-id="44600-136">O recurso **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44600-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="44600-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44600-137">Property name</span></span>      | <span data-ttu-id="44600-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="44600-138">Type</span></span>                       | <span data-ttu-id="44600-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="44600-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="44600-140">title</span><span class="sxs-lookup"><span data-stu-id="44600-140">title</span></span>              | <span data-ttu-id="44600-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44600-141">string</span></span>                     | <span data-ttu-id="44600-142">O título da página.</span><span class="sxs-lookup"><span data-stu-id="44600-142">The title of the page.</span></span>
| <span data-ttu-id="44600-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="44600-143">pageLayout</span></span>         | <span data-ttu-id="44600-144">string</span><span class="sxs-lookup"><span data-stu-id="44600-144">string</span></span>                     | <span data-ttu-id="44600-145">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="44600-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="44600-146">webParts</span><span class="sxs-lookup"><span data-stu-id="44600-146">webParts</span></span>           | <span data-ttu-id="44600-147">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="44600-147">[webPart][]</span></span>                | <span data-ttu-id="44600-148">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="44600-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="44600-149">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="44600-149">Authoring Metadata</span></span>

<span data-ttu-id="44600-150">O recurso **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="44600-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="44600-151">A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.</span><span class="sxs-lookup"><span data-stu-id="44600-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="44600-152">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44600-152">Property name</span></span>          | <span data-ttu-id="44600-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="44600-153">Type</span></span>                   | <span data-ttu-id="44600-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="44600-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="44600-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="44600-155">publishingState</span></span>        | <span data-ttu-id="44600-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="44600-156">[publicationFacet][]</span></span>   | <span data-ttu-id="44600-157">O status de publicação e a versão do MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="44600-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="44600-158">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="44600-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="44600-159">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="44600-159">Property name</span></span>        | <span data-ttu-id="44600-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="44600-160">Type</span></span>              | <span data-ttu-id="44600-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="44600-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="44600-162">id</span><span class="sxs-lookup"><span data-stu-id="44600-162">id</span></span>                   | <span data-ttu-id="44600-163">string</span><span class="sxs-lookup"><span data-stu-id="44600-163">string</span></span>            | <span data-ttu-id="44600-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="44600-166">name</span><span class="sxs-lookup"><span data-stu-id="44600-166">name</span></span>                 | <span data-ttu-id="44600-167">string</span><span class="sxs-lookup"><span data-stu-id="44600-167">string</span></span>            | <span data-ttu-id="44600-168">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="44600-168">The name / title of the item.</span></span>
| <span data-ttu-id="44600-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="44600-169">createdBy</span></span>            | <span data-ttu-id="44600-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="44600-170">[identitySet][]</span></span>   | <span data-ttu-id="44600-171">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="44600-171">Identity of the creator of this item.</span></span> <span data-ttu-id="44600-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-172">Read-only.</span></span>
| <span data-ttu-id="44600-173">eTag</span><span class="sxs-lookup"><span data-stu-id="44600-173">eTag</span></span>                 | <span data-ttu-id="44600-174">string</span><span class="sxs-lookup"><span data-stu-id="44600-174">string</span></span>            | <span data-ttu-id="44600-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="44600-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="44600-177">lastModifiedBy</span></span>       | <span data-ttu-id="44600-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="44600-178">[identitySet][]</span></span>   | <span data-ttu-id="44600-179">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="44600-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="44600-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-180">Read-only.</span></span>
| <span data-ttu-id="44600-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44600-181">lastModifiedDateTime</span></span> | <span data-ttu-id="44600-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44600-182">DateTimeOffset</span></span>    | <span data-ttu-id="44600-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="44600-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="44600-185">parentReference</span></span>      | <span data-ttu-id="44600-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="44600-186">[itemReference][]</span></span> | <span data-ttu-id="44600-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="44600-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="44600-189">webUrl</span></span>               | <span data-ttu-id="44600-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="44600-190">string (url)</span></span>      | <span data-ttu-id="44600-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="44600-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="44600-193">Relações</span><span class="sxs-lookup"><span data-stu-id="44600-193">Relationships</span></span>

<span data-ttu-id="44600-194">O recurso **sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="44600-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
