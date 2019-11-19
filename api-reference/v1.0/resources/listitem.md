---
author: JeremyKelley
ms.author: JeremyKelley
title: recurso listItem
description: Representa um item em uma lista do sharepoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e9a9010e8700d7e6ebd6a2e3d030fba7cab79f83
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703760"
---
# <a name="listitem-resource"></a><span data-ttu-id="f921c-103">recurso listItem</span><span class="sxs-lookup"><span data-stu-id="f921c-103">listItem resource</span></span>

<span data-ttu-id="f921c-104">Representa um item em uma **[lista][]** do Sharepoint.</span><span class="sxs-lookup"><span data-stu-id="f921c-104">Represents an item in a sharepoint list.</span></span>
<span data-ttu-id="f921c-105">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="f921c-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="f921c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f921c-106">Methods</span></span>

<span data-ttu-id="f921c-107">Os métodos a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="f921c-107">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="f921c-108">Todos os exemplos são relativos a uma **[lista][]**:`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="f921c-108">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="f921c-109">Método</span><span class="sxs-lookup"><span data-stu-id="f921c-109">Method</span></span>                    | <span data-ttu-id="f921c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f921c-110">Return Type</span></span> | <span data-ttu-id="f921c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f921c-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="f921c-112">[Get][]</span><span class="sxs-lookup"><span data-stu-id="f921c-112">[Get][]</span></span>                   | <span data-ttu-id="f921c-113">listItem</span><span class="sxs-lookup"><span data-stu-id="f921c-113">listItem</span></span>| <span data-ttu-id="f921c-114">Obter um item em uma lista.</span><span class="sxs-lookup"><span data-stu-id="f921c-114">Get an item in a list.</span></span>
| <span data-ttu-id="f921c-115">[Obter valores de coluna][Obter]</span><span class="sxs-lookup"><span data-stu-id="f921c-115">[Get column values][Get]</span></span>       | <span data-ttu-id="f921c-116">listItem</span><span class="sxs-lookup"><span data-stu-id="f921c-116">listItem</span></span> | <span data-ttu-id="f921c-117">Obter valores de coluna de listItem.</span><span class="sxs-lookup"><span data-stu-id="f921c-117">Get column values from listItem.</span></span>
| <span data-ttu-id="f921c-118">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="f921c-118">[Get analytics][]</span></span>              | <span data-ttu-id="f921c-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="f921c-119">[itemAnalytics][]</span></span>| <span data-ttu-id="f921c-120">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="f921c-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="f921c-121">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="f921c-121">[Get activities by interval][]</span></span> | <span data-ttu-id="f921c-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="f921c-122">[itemActivityStat][]</span></span>| <span data-ttu-id="f921c-123">Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="f921c-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="f921c-124">[Criar][]</span><span class="sxs-lookup"><span data-stu-id="f921c-124">[Create][]</span></span>                     | <span data-ttu-id="f921c-125">listItem</span><span class="sxs-lookup"><span data-stu-id="f921c-125">listItem</span></span> | <span data-ttu-id="f921c-126">Criar um novo listItem em uma lista.</span><span class="sxs-lookup"><span data-stu-id="f921c-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="f921c-127">[Excluir][]</span><span class="sxs-lookup"><span data-stu-id="f921c-127">[Delete][]</span></span>                     | <span data-ttu-id="f921c-128">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="f921c-128">No Content</span></span> | <span data-ttu-id="f921c-129">Remove um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="f921c-129">Removes an item from a list.</span></span>
| <span data-ttu-id="f921c-130">[Atualizar][]</span><span class="sxs-lookup"><span data-stu-id="f921c-130">[Update][]</span></span>                     | <span data-ttu-id="f921c-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="f921c-131">[fieldValueSet][]</span></span>| <span data-ttu-id="f921c-132">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="f921c-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="f921c-133">[Atualizar valores de coluna][Atualizar]</span><span class="sxs-lookup"><span data-stu-id="f921c-133">[Update column values][Update]</span></span> | <span data-ttu-id="f921c-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="f921c-134">[fieldValueSet][]</span></span>| <span data-ttu-id="f921c-135">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="f921c-135">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="f921c-144">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f921c-144">Properties</span></span>

<span data-ttu-id="f921c-145">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="f921c-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="f921c-146">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f921c-146">Property name</span></span> | <span data-ttu-id="f921c-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="f921c-147">Type</span></span>                | <span data-ttu-id="f921c-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="f921c-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="f921c-149">contentType</span><span class="sxs-lookup"><span data-stu-id="f921c-149">contentType</span></span>   | <span data-ttu-id="f921c-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="f921c-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="f921c-151">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="f921c-151">The content type of this list item</span></span>

<span data-ttu-id="f921c-152">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="f921c-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="f921c-153">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f921c-153">Property name</span></span>        | <span data-ttu-id="f921c-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="f921c-154">Type</span></span>              | <span data-ttu-id="f921c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="f921c-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="f921c-156">id</span><span class="sxs-lookup"><span data-stu-id="f921c-156">id</span></span>                   | <span data-ttu-id="f921c-157">string</span><span class="sxs-lookup"><span data-stu-id="f921c-157">string</span></span>            | <span data-ttu-id="f921c-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="f921c-160">name</span><span class="sxs-lookup"><span data-stu-id="f921c-160">name</span></span>                 | <span data-ttu-id="f921c-161">string</span><span class="sxs-lookup"><span data-stu-id="f921c-161">string</span></span>            | <span data-ttu-id="f921c-162">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="f921c-162">The name / title of the item.</span></span>
| <span data-ttu-id="f921c-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="f921c-163">createdBy</span></span>            | <span data-ttu-id="f921c-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f921c-164">[identitySet][]</span></span>   | <span data-ttu-id="f921c-165">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="f921c-165">Identity of the creator of this item.</span></span> <span data-ttu-id="f921c-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-166">Read-only.</span></span>
| <span data-ttu-id="f921c-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f921c-167">createdDateTime</span></span>      | <span data-ttu-id="f921c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f921c-168">DateTimeOffset</span></span>    | <span data-ttu-id="f921c-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="f921c-171">description</span><span class="sxs-lookup"><span data-stu-id="f921c-171">description</span></span>          | <span data-ttu-id="f921c-172">string</span><span class="sxs-lookup"><span data-stu-id="f921c-172">string</span></span>            | <span data-ttu-id="f921c-173">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="f921c-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="f921c-174">eTag</span><span class="sxs-lookup"><span data-stu-id="f921c-174">eTag</span></span>                 | <span data-ttu-id="f921c-175">string</span><span class="sxs-lookup"><span data-stu-id="f921c-175">string</span></span>            | <span data-ttu-id="f921c-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="f921c-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f921c-178">lastModifiedBy</span></span>       | <span data-ttu-id="f921c-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="f921c-179">[identitySet][]</span></span>   | <span data-ttu-id="f921c-180">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="f921c-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="f921c-181">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-181">Read-only.</span></span>
| <span data-ttu-id="f921c-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f921c-182">lastModifiedDateTime</span></span> | <span data-ttu-id="f921c-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f921c-183">DateTimeOffset</span></span>    | <span data-ttu-id="f921c-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="f921c-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="f921c-186">parentReference</span></span>      | <span data-ttu-id="f921c-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="f921c-187">[itemReference][]</span></span> | <span data-ttu-id="f921c-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="f921c-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="f921c-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="f921c-190">sharepointIds</span></span>        | <span data-ttu-id="f921c-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="f921c-191">[sharepointIds][]</span></span> | <span data-ttu-id="f921c-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="f921c-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="f921c-194">webUrl</span></span>               | <span data-ttu-id="f921c-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="f921c-195">string (url)</span></span>      | <span data-ttu-id="f921c-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f921c-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="f921c-198">Relações</span><span class="sxs-lookup"><span data-stu-id="f921c-198">Relationships</span></span>

 <span data-ttu-id="f921c-199">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="f921c-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="f921c-200">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="f921c-200">Relationship name</span></span> | <span data-ttu-id="f921c-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="f921c-201">Type</span></span>                           | <span data-ttu-id="f921c-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="f921c-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="f921c-203">activities</span><span class="sxs-lookup"><span data-stu-id="f921c-203">activities</span></span>        | <span data-ttu-id="f921c-204">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="f921c-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="f921c-205">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="f921c-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="f921c-206">análise</span><span class="sxs-lookup"><span data-stu-id="f921c-206">analytics</span></span>         | <span data-ttu-id="f921c-207">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="f921c-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="f921c-208">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="f921c-208">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="f921c-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="f921c-209">driveItem</span></span>         | <span data-ttu-id="f921c-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="f921c-210">[driveItem][]</span></span>                  | <span data-ttu-id="f921c-211">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="f921c-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="f921c-212">campos</span><span class="sxs-lookup"><span data-stu-id="f921c-212">fields</span></span>            | <span data-ttu-id="f921c-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="f921c-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="f921c-214">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="f921c-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="f921c-215">versões</span><span class="sxs-lookup"><span data-stu-id="f921c-215">versions</span></span>          | <span data-ttu-id="f921c-216">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="f921c-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="f921c-217">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="f921c-217">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="f921c-229">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f921c-229">JSON representation</span></span>

<span data-ttu-id="f921c-230">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="f921c-230">Here is a JSON representation of a **listItem** resource.</span></span>

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
