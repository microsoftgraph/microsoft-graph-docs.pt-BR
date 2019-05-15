---
author: JeremyKelley
ms.author: JeremyKelley
title: recurso listItem
description: Este recurso representa um item em uma lista do sharepoint.
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 873ad5961c9cadb444c6fe9f2afec69853cc5d85
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968797"
---
# <a name="listitem-resource"></a><span data-ttu-id="6f3a2-103">recurso listItem</span><span class="sxs-lookup"><span data-stu-id="6f3a2-103">ListItem resource</span></span>

<span data-ttu-id="6f3a2-104">Este recurso representa um item em uma **[list][]** do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="6f3a2-105">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="6f3a2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6f3a2-106">Methods</span></span>

<span data-ttu-id="6f3a2-107">Os métodos a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="6f3a2-108">Todos os exemplos são relativos a uma **[lista][]**:`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="6f3a2-109">Método</span><span class="sxs-lookup"><span data-stu-id="6f3a2-109">Method</span></span>                    | <span data-ttu-id="6f3a2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6f3a2-110">Return Type</span></span> | <span data-ttu-id="6f3a2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f3a2-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="6f3a2-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-112">[Get][]</span></span>                   | <span data-ttu-id="6f3a2-113">lisItem</span><span class="sxs-lookup"><span data-stu-id="6f3a2-113">lisItem</span></span>| <span data-ttu-id="6f3a2-114">Obter um item em uma lista.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-114">Get an item in a list</span></span>
| <span data-ttu-id="6f3a2-115">[Obter valores de coluna][Obter]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-115">[Get column values][Get]</span></span>       | <span data-ttu-id="6f3a2-116">listItem</span><span class="sxs-lookup"><span data-stu-id="6f3a2-116">listItem</span></span> | <span data-ttu-id="6f3a2-117">Obter valores de coluna de listItem.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-117">Get column values from listItem.</span></span>
| <span data-ttu-id="6f3a2-118">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-118">[Get analytics][]</span></span>              | <span data-ttu-id="6f3a2-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-119">[itemAnalytics][]</span></span>| <span data-ttu-id="6f3a2-120">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="6f3a2-121">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-121">[Get activities by interval][]</span></span> | <span data-ttu-id="6f3a2-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-122">[itemActivityStat][]</span></span>| <span data-ttu-id="6f3a2-123">Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="6f3a2-124">[Criar][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-124">[Create][]</span></span>                     | <span data-ttu-id="6f3a2-125">listItem</span><span class="sxs-lookup"><span data-stu-id="6f3a2-125">listItem</span></span> | <span data-ttu-id="6f3a2-126">Criar um novo listItem em uma lista.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="6f3a2-127">[Excluir][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-127">[Delete][]</span></span>                     | <span data-ttu-id="6f3a2-128">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="6f3a2-128">204 No Content</span></span> | <span data-ttu-id="6f3a2-129">Remove um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-129">Removes an item from a list.</span></span>
| <span data-ttu-id="6f3a2-130">[Atualizar][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-130">[Update][]</span></span>                     | <span data-ttu-id="6f3a2-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-131">[fieldValueSet][]</span></span>| <span data-ttu-id="6f3a2-132">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="6f3a2-133">[Atualizar valores de coluna][Atualizar]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-133">[Update column values][Update]</span></span> | <span data-ttu-id="6f3a2-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-134">[fieldValueSet][]</span></span>| <span data-ttu-id="6f3a2-135">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-135">Update column values on a listItem.</span></span>

[Obter]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[Excluir]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Atualizar]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a><span data-ttu-id="6f3a2-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6f3a2-144">Properties</span></span>

<span data-ttu-id="6f3a2-145">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="6f3a2-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6f3a2-146">Property name</span></span> | <span data-ttu-id="6f3a2-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f3a2-147">Type</span></span>                | <span data-ttu-id="6f3a2-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f3a2-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="6f3a2-149">contentType</span><span class="sxs-lookup"><span data-stu-id="6f3a2-149">contentType</span></span>   | <span data-ttu-id="6f3a2-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="6f3a2-151">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="6f3a2-151">The content type of this list item</span></span>

<span data-ttu-id="6f3a2-152">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="6f3a2-153">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="6f3a2-153">Property name</span></span>        | <span data-ttu-id="6f3a2-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f3a2-154">Type</span></span>              | <span data-ttu-id="6f3a2-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f3a2-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="6f3a2-156">id</span><span class="sxs-lookup"><span data-stu-id="6f3a2-156">id</span></span>                   | <span data-ttu-id="6f3a2-157">string</span><span class="sxs-lookup"><span data-stu-id="6f3a2-157">string</span></span>            | <span data-ttu-id="6f3a2-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="6f3a2-160">name</span><span class="sxs-lookup"><span data-stu-id="6f3a2-160">name</span></span>                 | <span data-ttu-id="6f3a2-161">string</span><span class="sxs-lookup"><span data-stu-id="6f3a2-161">string</span></span>            | <span data-ttu-id="6f3a2-162">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-162">The name / title of the item.</span></span>
| <span data-ttu-id="6f3a2-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="6f3a2-163">createdBy</span></span>            | <span data-ttu-id="6f3a2-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-164">[identitySet][]</span></span>   | <span data-ttu-id="6f3a2-165">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-165">Identity of the creator of this item.</span></span> <span data-ttu-id="6f3a2-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-166">Read-only.</span></span>
| <span data-ttu-id="6f3a2-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f3a2-167">createdDateTime</span></span>      | <span data-ttu-id="6f3a2-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f3a2-168">DateTimeOffset</span></span>    | <span data-ttu-id="6f3a2-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="6f3a2-171">description</span><span class="sxs-lookup"><span data-stu-id="6f3a2-171">description</span></span>          | <span data-ttu-id="6f3a2-172">string</span><span class="sxs-lookup"><span data-stu-id="6f3a2-172">string</span></span>            | <span data-ttu-id="6f3a2-173">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="6f3a2-174">eTag</span><span class="sxs-lookup"><span data-stu-id="6f3a2-174">eTag</span></span>                 | <span data-ttu-id="6f3a2-175">string</span><span class="sxs-lookup"><span data-stu-id="6f3a2-175">string</span></span>            | <span data-ttu-id="6f3a2-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="6f3a2-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6f3a2-178">lastModifiedBy</span></span>       | <span data-ttu-id="6f3a2-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-179">[identitySet][]</span></span>   | <span data-ttu-id="6f3a2-180">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="6f3a2-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-181">Read-only.</span></span>
| <span data-ttu-id="6f3a2-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6f3a2-182">lastModifiedDateTime</span></span> | <span data-ttu-id="6f3a2-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f3a2-183">DateTimeOffset</span></span>    | <span data-ttu-id="6f3a2-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="6f3a2-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="6f3a2-186">parentReference</span></span>      | <span data-ttu-id="6f3a2-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-187">[itemReference][]</span></span> | <span data-ttu-id="6f3a2-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="6f3a2-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="6f3a2-190">sharepointIds</span></span>        | <span data-ttu-id="6f3a2-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-191">[sharepointIds][]</span></span> | <span data-ttu-id="6f3a2-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="6f3a2-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="6f3a2-194">webUrl</span></span>               | <span data-ttu-id="6f3a2-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="6f3a2-195">string (url)</span></span>      | <span data-ttu-id="6f3a2-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="6f3a2-198">Relações</span><span class="sxs-lookup"><span data-stu-id="6f3a2-198">Relationships</span></span>

 <span data-ttu-id="6f3a2-199">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="6f3a2-200">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="6f3a2-200">Relationship name</span></span> | <span data-ttu-id="6f3a2-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="6f3a2-201">Type</span></span>                           | <span data-ttu-id="6f3a2-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="6f3a2-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="6f3a2-203">activities</span><span class="sxs-lookup"><span data-stu-id="6f3a2-203">activities</span></span>        | <span data-ttu-id="6f3a2-204">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="6f3a2-205">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="6f3a2-206">análise</span><span class="sxs-lookup"><span data-stu-id="6f3a2-206">analytics</span></span>         | <span data-ttu-id="6f3a2-207">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="6f3a2-208">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-208">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="6f3a2-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="6f3a2-209">driveItem</span></span>         | <span data-ttu-id="6f3a2-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-210">[driveItem][]</span></span>                  | <span data-ttu-id="6f3a2-211">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="6f3a2-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="6f3a2-212">campos</span><span class="sxs-lookup"><span data-stu-id="6f3a2-212">fields</span></span>            | <span data-ttu-id="6f3a2-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="6f3a2-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="6f3a2-214">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="6f3a2-215">versões</span><span class="sxs-lookup"><span data-stu-id="6f3a2-215">versions</span></span>          | <span data-ttu-id="6f3a2-216">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="6f3a2-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="6f3a2-217">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-217">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

## <a name="json-representation"></a><span data-ttu-id="6f3a2-229">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6f3a2-229">JSON representation</span></span>

<span data-ttu-id="6f3a2-230">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="6f3a2-230">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
