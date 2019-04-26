---
author: rahmit
ms.author: rahmit
ms.date: 03/15/2018
title: SitePage
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6a9192423c4caf47913029e3671e975884533333
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343063"
---
# <a name="sitepage-resource"></a><span data-ttu-id="7697c-102">recurso sitePage</span><span class="sxs-lookup"><span data-stu-id="7697c-102">sitePage resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7697c-103">Esse recurso representa uma página na [lista][]SitePages.</span><span class="sxs-lookup"><span data-stu-id="7697c-103">This resource represents a page in the SitePages [list][].</span></span>
<span data-ttu-id="7697c-104">Ele contém o título, o layout e uma coleção de [WebPart][]s.</span><span class="sxs-lookup"><span data-stu-id="7697c-104">It contains the title, layout, and a collection of [webPart][]s.</span></span>

## <a name="tasks-on-a-page"></a><span data-ttu-id="7697c-105">Tarefas em uma página</span><span class="sxs-lookup"><span data-stu-id="7697c-105">Tasks on a page</span></span>

<span data-ttu-id="7697c-106">As tarefas a seguir estão disponíveis para recursos do **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="7697c-106">The following tasks are available for **sitePage** resources.</span></span>
<span data-ttu-id="7697c-107">Todos os exemplos abaixo são relativos a um [site][], por `https://graph.microsoft.com/{api-version}/sites/{site-id}`exemplo:.</span><span class="sxs-lookup"><span data-stu-id="7697c-107">All examples below are relative to a [site][], eg: `https://graph.microsoft.com/{api-version}/sites/{site-id}`.</span></span>

| <span data-ttu-id="7697c-108">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="7697c-108">Common task</span></span>                     | <span data-ttu-id="7697c-109">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="7697c-109">HTTP method</span></span>
|:--------------------------------|:------------------------------
| <span data-ttu-id="7697c-110">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="7697c-110">[List pages][]</span></span>                  | <span data-ttu-id="7697c-111">OBTER/Pages</span><span class="sxs-lookup"><span data-stu-id="7697c-111">GET /pages</span></span>
| <span data-ttu-id="7697c-112">[Obter página][]</span><span class="sxs-lookup"><span data-stu-id="7697c-112">[Get page][]</span></span>                    | <span data-ttu-id="7697c-113">OBTER/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="7697c-113">GET /pages/{page-id}</span></span>
| <span data-ttu-id="7697c-114">[Criar][]</span><span class="sxs-lookup"><span data-stu-id="7697c-114">[Create][]</span></span>                      | <span data-ttu-id="7697c-115">POSTAR/Pages</span><span class="sxs-lookup"><span data-stu-id="7697c-115">POST /pages</span></span>
| <span data-ttu-id="7697c-116">[Delete][]</span><span class="sxs-lookup"><span data-stu-id="7697c-116">[Delete][]</span></span>                      | <span data-ttu-id="7697c-117">EXCLUIR/Pages/{Page-ID}</span><span class="sxs-lookup"><span data-stu-id="7697c-117">DELETE /pages/{page-id}</span></span>
| <span data-ttu-id="7697c-118">[Publish][]</span><span class="sxs-lookup"><span data-stu-id="7697c-118">[Publish][]</span></span>                     | <span data-ttu-id="7697c-119">POSTAR/Pages/{Page-ID}/Publish</span><span class="sxs-lookup"><span data-stu-id="7697c-119">POST /pages/{page-id}/publish</span></span>

[List pages]: ../api/sitepage-list.md
[Obter página]: ../api/sitepage-get.md
[Get page]: ../api/sitepage-get.md
[Create]: ../api/sitepage-create.md
[Delete]: ../api/sitepage-delete.md
[Publish]: ../api/sitepage-publish.md

## <a name="json-representation"></a><span data-ttu-id="7697c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7697c-125">JSON representation</span></span>

<span data-ttu-id="7697c-126">Veja a seguir uma representação JSON de um recurso **sitePage** .</span><span class="sxs-lookup"><span data-stu-id="7697c-126">Here is a JSON representation of a **sitePage** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7697c-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7697c-127">Properties</span></span>

<span data-ttu-id="7697c-128">O recurso **sitePage** tem as propriedades a seguir.</span><span class="sxs-lookup"><span data-stu-id="7697c-128">The **sitePage** resource has the following properties.</span></span>

| <span data-ttu-id="7697c-129">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7697c-129">Property name</span></span>    | <span data-ttu-id="7697c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7697c-130">Type</span></span>                         | <span data-ttu-id="7697c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7697c-131">Description</span></span>
|:-----------------|:-----------------------------|:---------------------------
| <span data-ttu-id="7697c-132">contentType</span><span class="sxs-lookup"><span data-stu-id="7697c-132">contentType</span></span>      | <span data-ttu-id="7697c-133">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="7697c-133">[contentTypeInfo][]</span></span>          | <span data-ttu-id="7697c-134">O tipo de conteúdo da página.</span><span class="sxs-lookup"><span data-stu-id="7697c-134">The content type of the page.</span></span>

## <a name="page-content"></a><span data-ttu-id="7697c-135">Conteúdo da página</span><span class="sxs-lookup"><span data-stu-id="7697c-135">Page Content</span></span>

<span data-ttu-id="7697c-136">O recurso **sitePage** tem os seguintes campos de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7697c-136">The **sitePage** resource has the following content fields.</span></span>

| <span data-ttu-id="7697c-137">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7697c-137">Property name</span></span>      | <span data-ttu-id="7697c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="7697c-138">Type</span></span>                       | <span data-ttu-id="7697c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="7697c-139">Description</span></span>
|:-------------------|:---------------------------|:---------------------------
| <span data-ttu-id="7697c-140">title</span><span class="sxs-lookup"><span data-stu-id="7697c-140">title</span></span>              | <span data-ttu-id="7697c-141">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7697c-141">string</span></span>                     | <span data-ttu-id="7697c-142">O título da página.</span><span class="sxs-lookup"><span data-stu-id="7697c-142">The title of the page.</span></span>
| <span data-ttu-id="7697c-143">pageLayout</span><span class="sxs-lookup"><span data-stu-id="7697c-143">pageLayout</span></span>         | <span data-ttu-id="7697c-144">string</span><span class="sxs-lookup"><span data-stu-id="7697c-144">string</span></span>                     | <span data-ttu-id="7697c-145">O nome do layout de página da página.</span><span class="sxs-lookup"><span data-stu-id="7697c-145">The name of the page layout of the page.</span></span>
| <span data-ttu-id="7697c-146">webParts</span><span class="sxs-lookup"><span data-stu-id="7697c-146">webParts</span></span>           | <span data-ttu-id="7697c-147">[webPart][]</span><span class="sxs-lookup"><span data-stu-id="7697c-147">[webPart][]</span></span>                | <span data-ttu-id="7697c-148">As Web Parts na página.</span><span class="sxs-lookup"><span data-stu-id="7697c-148">The web parts on the page.</span></span>

## <a name="authoring-metadata"></a><span data-ttu-id="7697c-149">Criação de metadados</span><span class="sxs-lookup"><span data-stu-id="7697c-149">Authoring Metadata</span></span>

<span data-ttu-id="7697c-150">O recurso **sitePage** tem os seguintes metadados relacionados a criação.</span><span class="sxs-lookup"><span data-stu-id="7697c-150">The **sitePage** resource has the following authoring-related metadata.</span></span> <span data-ttu-id="7697c-151">A propriedade publishingstate refletirá o estado de criação da página, como check-out ou publicada.</span><span class="sxs-lookup"><span data-stu-id="7697c-151">The publishingState property will reflect the page authoring state like checked out or published.</span></span>

| <span data-ttu-id="7697c-152">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7697c-152">Property name</span></span>          | <span data-ttu-id="7697c-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="7697c-153">Type</span></span>                   | <span data-ttu-id="7697c-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="7697c-154">Description</span></span>
|:-----------------------|:-----------------------|:---------------------------
| <span data-ttu-id="7697c-155">publishingState</span><span class="sxs-lookup"><span data-stu-id="7697c-155">publishingState</span></span>        | <span data-ttu-id="7697c-156">[publicationFacet][]</span><span class="sxs-lookup"><span data-stu-id="7697c-156">[publicationFacet][]</span></span>   | <span data-ttu-id="7697c-157">O status de publicação e a versão do MM.mm da página.</span><span class="sxs-lookup"><span data-stu-id="7697c-157">The publishing status and the MM.mm version of the page.</span></span>

<span data-ttu-id="7697c-158">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="7697c-158">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="7697c-159">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7697c-159">Property name</span></span>        | <span data-ttu-id="7697c-160">Tipo</span><span class="sxs-lookup"><span data-stu-id="7697c-160">Type</span></span>              | <span data-ttu-id="7697c-161">Descrição</span><span class="sxs-lookup"><span data-stu-id="7697c-161">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="7697c-162">id</span><span class="sxs-lookup"><span data-stu-id="7697c-162">id</span></span>                   | <span data-ttu-id="7697c-163">string</span><span class="sxs-lookup"><span data-stu-id="7697c-163">string</span></span>            | <span data-ttu-id="7697c-p104">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="7697c-166">name</span><span class="sxs-lookup"><span data-stu-id="7697c-166">name</span></span>                 | <span data-ttu-id="7697c-167">string</span><span class="sxs-lookup"><span data-stu-id="7697c-167">string</span></span>            | <span data-ttu-id="7697c-168">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="7697c-168">The name / title of the item.</span></span>
| <span data-ttu-id="7697c-169">createdBy</span><span class="sxs-lookup"><span data-stu-id="7697c-169">createdBy</span></span>            | <span data-ttu-id="7697c-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7697c-170">[identitySet][]</span></span>   | <span data-ttu-id="7697c-171">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="7697c-171">Identity of the creator of this item.</span></span> <span data-ttu-id="7697c-172">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-172">Read-only.</span></span>
| <span data-ttu-id="7697c-173">eTag</span><span class="sxs-lookup"><span data-stu-id="7697c-173">eTag</span></span>                 | <span data-ttu-id="7697c-174">string</span><span class="sxs-lookup"><span data-stu-id="7697c-174">string</span></span>            | <span data-ttu-id="7697c-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-p106">ETag for the item. Read-only.</span></span>
| <span data-ttu-id="7697c-177">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7697c-177">lastModifiedBy</span></span>       | <span data-ttu-id="7697c-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7697c-178">[identitySet][]</span></span>   | <span data-ttu-id="7697c-179">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="7697c-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="7697c-180">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-180">Read-only.</span></span>
| <span data-ttu-id="7697c-181">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7697c-181">lastModifiedDateTime</span></span> | <span data-ttu-id="7697c-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7697c-182">DateTimeOffset</span></span>    | <span data-ttu-id="7697c-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7697c-185">parentReference</span><span class="sxs-lookup"><span data-stu-id="7697c-185">parentReference</span></span>      | <span data-ttu-id="7697c-186">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7697c-186">[itemReference][]</span></span> | <span data-ttu-id="7697c-p109">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7697c-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="7697c-189">webUrl</span></span>               | <span data-ttu-id="7697c-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="7697c-190">string (url)</span></span>      | <span data-ttu-id="7697c-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7697c-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="7697c-193">Relações</span><span class="sxs-lookup"><span data-stu-id="7697c-193">Relationships</span></span>

<span data-ttu-id="7697c-194">O recurso **sitePage** não tem relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="7697c-194">The **sitePage** resource does not have relationships to other resources.</span></span>

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
