---
author: rahmit
description: Esse recurso representa uma página na lista SitePages.
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: d92a78ff73854d465ba8363b7bddff66be6bffc4
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953610"
---
# <a name="sitepage-resource"></a><span data-ttu-id="df185-103">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="df185-103">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df185-104">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="df185-104">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="df185-105">Ele contém o título, o layout e uma coleção de [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="df185-105">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="df185-106">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="df185-106">Tasks on a page</span></span>

<span data-ttu-id="df185-107">As tarefas a seguir estão disponíveis para recursos do **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="df185-107">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="df185-108">Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.</span><span class="sxs-lookup"><span data-stu-id="df185-108">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="df185-109">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="df185-109">Common task</span></span>                     | <span data-ttu-id="df185-110">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="df185-110">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="df185-111">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="df185-111">[List pages][]</span></span>                  | <span data-ttu-id="df185-112">OBTER/Pages</span><span class="sxs-lookup"><span data-stu-id="df185-112">GET /pages</span></span>
| <span data-ttu-id="df185-113">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="df185-113">[Get page][]</span></span>                    | <span data-ttu-id="df185-114">OBTER/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="df185-114">GET /pages/{page-id}</span></span>
| <span data-ttu-id="df185-115">[Create][]</span><span class="sxs-lookup"><span data-stu-id="df185-115">[Create][]</span></span>                      | <span data-ttu-id="df185-116">POSTAR/Pages</span><span class="sxs-lookup"><span data-stu-id="df185-116">POST /pages</span></span>
| <span data-ttu-id="df185-117">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="df185-117">[Delete][]</span></span>                      | <span data-ttu-id="df185-118">EXCLUIR/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="df185-118">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="df185-119">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="df185-119">[Publish][]</span></span>                     | <span data-ttu-id="df185-120">POSTAR/Pages/{Page-ID}/Publish</span><span class="sxs-lookup"><span data-stu-id="df185-120">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="df185-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df185-126">JSON representation</span></span>

<span data-ttu-id="df185-127">Veja a seguir uma representação JSON de um recurso **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="df185-127">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="df185-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df185-128">Properties</span></span>

<span data-ttu-id="df185-129">O recurso **sitePage** tem as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="df185-129">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="df185-130">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="df185-130">Property name</span></span>    | <span data-ttu-id="df185-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df185-131">Type</span></span>                         | <span data-ttu-id="df185-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df185-132">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="df185-133">contentType</span><span class="sxs-lookup"><span data-stu-id="df185-133">contentType</span></span>      | <span data-ttu-id="df185-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="df185-134">[contentTypeInfo][]</span></span>          | <span data-ttu-id="df185-135">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="df185-135">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="df185-136">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="df185-136">Page Content</span></span>

<span data-ttu-id="df185-137">O recurso **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="df185-137">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="df185-138">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="df185-138">Property name</span></span>      | <span data-ttu-id="df185-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="df185-139">Type</span></span>                       | <span data-ttu-id="df185-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="df185-140">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="df185-141">title</span><span class="sxs-lookup"><span data-stu-id="df185-141">title</span></span>              | <span data-ttu-id="df185-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df185-142">string</span></span>                     | <span data-ttu-id="df185-143">O título da página.</span><span class="sxs-lookup"><span data-stu-id="df185-143">The title of the page.</span></span>
| <span data-ttu-id="df185-144">pageLayout</span><span class="sxs-lookup"><span data-stu-id="df185-144">pageLayout</span></span>         | <span data-ttu-id="df185-145">string</span><span class="sxs-lookup"><span data-stu-id="df185-145">string</span></span>                     | <span data-ttu-id="df185-146">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="df185-146">The name of the page layout of the page.</span></span>
| <span data-ttu-id="df185-147">webParts</span><span class="sxs-lookup"><span data-stu-id="df185-147">webParts</span></span>           | <span data-ttu-id="df185-148">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="df185-148">[webPart][]</span></span>                | <span data-ttu-id="df185-149">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="df185-149">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="df185-150">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="df185-150">Authoring Metadata</span></span>

<span data-ttu-id="df185-151">O recurso **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="df185-151">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="df185-152">A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.</span><span class="sxs-lookup"><span data-stu-id="df185-152">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="df185-153">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="df185-153">Property name</span></span>          | <span data-ttu-id="df185-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="df185-154">Type</span></span>                   | <span data-ttu-id="df185-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="df185-155">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="df185-156">publishingState</span><span class="sxs-lookup"><span data-stu-id="df185-156">publishingState</span></span>        | <span data-ttu-id="df185-157">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="df185-157">[publicationFacet][]</span></span>   | <span data-ttu-id="df185-158">O status de publicação e a versão do MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="df185-158">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="df185-159">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="df185-159">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="df185-160">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="df185-160">Property name</span></span>        | <span data-ttu-id="df185-161">Tipo</span><span class="sxs-lookup"><span data-stu-id="df185-161">Type</span></span>              | <span data-ttu-id="df185-162">Descrição</span><span class="sxs-lookup"><span data-stu-id="df185-162">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="df185-163">id</span><span class="sxs-lookup"><span data-stu-id="df185-163">id</span></span>                   | <span data-ttu-id="df185-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df185-164">string</span></span>            | <span data-ttu-id="df185-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="df185-167">name</span><span class="sxs-lookup"><span data-stu-id="df185-167">name</span></span>                 | <span data-ttu-id="df185-168">string</span><span class="sxs-lookup"><span data-stu-id="df185-168">string</span></span>            | <span data-ttu-id="df185-169">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="df185-169">The name / title of the item.</span></span>
| <span data-ttu-id="df185-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="df185-170">createdBy</span></span>            | <span data-ttu-id="df185-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df185-171">[identitySet][]</span></span>   | <span data-ttu-id="df185-172">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="df185-172">Identity of the creator of this item.</span></span> <span data-ttu-id="df185-173">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-173">Read-only.</span></span>
| <span data-ttu-id="df185-174">eTag</span><span class="sxs-lookup"><span data-stu-id="df185-174">eTag</span></span>                 | <span data-ttu-id="df185-175">string</span><span class="sxs-lookup"><span data-stu-id="df185-175">string</span></span>            | <span data-ttu-id="df185-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="df185-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="df185-178">lastModifiedBy</span></span>       | <span data-ttu-id="df185-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="df185-179">[identitySet][]</span></span>   | <span data-ttu-id="df185-180">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="df185-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="df185-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-181">Read-only.</span></span>
| <span data-ttu-id="df185-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df185-182">lastModifiedDateTime</span></span> | <span data-ttu-id="df185-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df185-183">DateTimeOffset</span></span>    | <span data-ttu-id="df185-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="df185-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="df185-186">parentReference</span></span>      | <span data-ttu-id="df185-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="df185-187">[itemReference][]</span></span> | <span data-ttu-id="df185-188">Informações do pai, se o item tiver um pai.</span><span class="sxs-lookup"><span data-stu-id="df185-188">Parent information, if the item has a parent.</span></span> <span data-ttu-id="df185-189">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-189">Read-only.</span></span>
| <span data-ttu-id="df185-190">webUrl</span><span class="sxs-lookup"><span data-stu-id="df185-190">webUrl</span></span>               | <span data-ttu-id="df185-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="df185-191">string (url)</span></span>      | <span data-ttu-id="df185-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="df185-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="df185-194">Relações</span><span class="sxs-lookup"><span data-stu-id="df185-194">Relationships</span></span>

<span data-ttu-id="df185-195">O recurso **sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="df185-195">The **sitePage** resource does not have relationships to other resources.</span></span>

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
