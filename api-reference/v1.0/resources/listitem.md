---
author: JeremyKelley
title: recurso listItem
description: Representa um item em uma lista do sharepoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7e9e7b00ee87127b7844d2d7208d63c8e4fb6af5
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714113"
---
# <a name="listitem-resource"></a><span data-ttu-id="750c6-103">recurso listItem</span><span class="sxs-lookup"><span data-stu-id="750c6-103">listItem resource</span></span>

<span data-ttu-id="750c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="750c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="750c6-105">Representa um item em uma [lista][] do Microsoft Office SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="750c6-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="750c6-106">Todos os itens em uma biblioteca de documentos do Microsoft Office SharePoint Online podem ser representados como um **listItem** ou um r[ecurso driveItem][].</span><span class="sxs-lookup"><span data-stu-id="750c6-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="750c6-107">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="750c6-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="750c6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="750c6-108">Methods</span></span>

<span data-ttu-id="750c6-109">Os métodos a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="750c6-109">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="750c6-110">Todos os exemplos são relativos a uma **[lista][]**:`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="750c6-110">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="750c6-111">Método</span><span class="sxs-lookup"><span data-stu-id="750c6-111">Method</span></span>                    | <span data-ttu-id="750c6-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="750c6-112">Return Type</span></span> | <span data-ttu-id="750c6-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="750c6-113">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="750c6-114">[Get][]</span><span class="sxs-lookup"><span data-stu-id="750c6-114">[Get][]</span></span>                   | <span data-ttu-id="750c6-115">listItem</span><span class="sxs-lookup"><span data-stu-id="750c6-115">listItem</span></span>| <span data-ttu-id="750c6-116">Obter um item em uma lista.</span><span class="sxs-lookup"><span data-stu-id="750c6-116">Get an item in a list.</span></span>
| <span data-ttu-id="750c6-117">[Obter valores de coluna][Obter]</span><span class="sxs-lookup"><span data-stu-id="750c6-117">[Get column values][Get]</span></span>       | <span data-ttu-id="750c6-118">listItem</span><span class="sxs-lookup"><span data-stu-id="750c6-118">listItem</span></span> | <span data-ttu-id="750c6-119">Obter valores de coluna de listItem.</span><span class="sxs-lookup"><span data-stu-id="750c6-119">Get column values from listItem.</span></span>
| <span data-ttu-id="750c6-120">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="750c6-120">[Get analytics][]</span></span>              | <span data-ttu-id="750c6-121">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="750c6-121">[itemAnalytics][]</span></span>| <span data-ttu-id="750c6-122">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="750c6-122">Get analytics for this resource.</span></span> 
| <span data-ttu-id="750c6-123">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="750c6-123">[Get activities by interval][]</span></span> | <span data-ttu-id="750c6-124">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="750c6-124">[itemActivityStat][]</span></span>| <span data-ttu-id="750c6-125">Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="750c6-125">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="750c6-126">[Criar][]</span><span class="sxs-lookup"><span data-stu-id="750c6-126">[Create][]</span></span>                     | <span data-ttu-id="750c6-127">listItem</span><span class="sxs-lookup"><span data-stu-id="750c6-127">listItem</span></span> | <span data-ttu-id="750c6-128">Criar um novo listItem em uma lista.</span><span class="sxs-lookup"><span data-stu-id="750c6-128">Create a new listItem in a list.</span></span>
| <span data-ttu-id="750c6-129">[Excluir][]</span><span class="sxs-lookup"><span data-stu-id="750c6-129">[Delete][]</span></span>                     | <span data-ttu-id="750c6-130">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="750c6-130">No Content</span></span> | <span data-ttu-id="750c6-131">Remove um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="750c6-131">Removes an item from a list.</span></span>
| <span data-ttu-id="750c6-132">[Atualizar][]</span><span class="sxs-lookup"><span data-stu-id="750c6-132">[Update][]</span></span>                     | <span data-ttu-id="750c6-133">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="750c6-133">[fieldValueSet][]</span></span>| <span data-ttu-id="750c6-134">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="750c6-134">Update the properties on a listItem.</span></span>
| <span data-ttu-id="750c6-135">[Atualizar valores de coluna][Atualizar]</span><span class="sxs-lookup"><span data-stu-id="750c6-135">[Update column values][Update]</span></span> | <span data-ttu-id="750c6-136">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="750c6-136">[fieldValueSet][]</span></span>| <span data-ttu-id="750c6-137">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="750c6-137">Update column values on a listItem.</span></span>

[Obter]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[Obter análises]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[Obter atividades por intervalo]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[Delete]: ../api/listitem-delete.md
[Atualizar]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a><span data-ttu-id="750c6-146">Propriedades</span><span class="sxs-lookup"><span data-stu-id="750c6-146">Properties</span></span>

<span data-ttu-id="750c6-147">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="750c6-147">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="750c6-148">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="750c6-148">Property name</span></span> | <span data-ttu-id="750c6-149">Tipo</span><span class="sxs-lookup"><span data-stu-id="750c6-149">Type</span></span>                | <span data-ttu-id="750c6-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="750c6-150">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="750c6-151">contentType</span><span class="sxs-lookup"><span data-stu-id="750c6-151">contentType</span></span>   | <span data-ttu-id="750c6-152">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="750c6-152">[contentTypeInfo][]</span></span> | <span data-ttu-id="750c6-153">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="750c6-153">The content type of this list item</span></span>

<span data-ttu-id="750c6-154">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="750c6-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="750c6-155">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="750c6-155">Property name</span></span>        | <span data-ttu-id="750c6-156">Tipo</span><span class="sxs-lookup"><span data-stu-id="750c6-156">Type</span></span>              | <span data-ttu-id="750c6-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="750c6-157">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="750c6-158">id</span><span class="sxs-lookup"><span data-stu-id="750c6-158">id</span></span>                   | <span data-ttu-id="750c6-159">string</span><span class="sxs-lookup"><span data-stu-id="750c6-159">string</span></span>            | <span data-ttu-id="750c6-p102">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="750c6-162">name</span><span class="sxs-lookup"><span data-stu-id="750c6-162">name</span></span>                 | <span data-ttu-id="750c6-163">string</span><span class="sxs-lookup"><span data-stu-id="750c6-163">string</span></span>            | <span data-ttu-id="750c6-164">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="750c6-164">The name / title of the item.</span></span>
| <span data-ttu-id="750c6-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="750c6-165">createdBy</span></span>            | <span data-ttu-id="750c6-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="750c6-166">[identitySet][]</span></span>   | <span data-ttu-id="750c6-167">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="750c6-167">Identity of the creator of this item.</span></span> <span data-ttu-id="750c6-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-168">Read-only.</span></span>
| <span data-ttu-id="750c6-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="750c6-169">createdDateTime</span></span>      | <span data-ttu-id="750c6-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="750c6-170">DateTimeOffset</span></span>    | <span data-ttu-id="750c6-p104">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="750c6-173">description</span><span class="sxs-lookup"><span data-stu-id="750c6-173">description</span></span>          | <span data-ttu-id="750c6-174">string</span><span class="sxs-lookup"><span data-stu-id="750c6-174">string</span></span>            | <span data-ttu-id="750c6-175">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="750c6-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="750c6-176">eTag</span><span class="sxs-lookup"><span data-stu-id="750c6-176">eTag</span></span>                 | <span data-ttu-id="750c6-177">string</span><span class="sxs-lookup"><span data-stu-id="750c6-177">string</span></span>            | <span data-ttu-id="750c6-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="750c6-180">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="750c6-180">lastModifiedBy</span></span>       | <span data-ttu-id="750c6-181">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="750c6-181">[identitySet][]</span></span>   | <span data-ttu-id="750c6-182">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="750c6-182">Identity of the last modifier of this item.</span></span> <span data-ttu-id="750c6-183">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-183">Read-only.</span></span>
| <span data-ttu-id="750c6-184">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="750c6-184">lastModifiedDateTime</span></span> | <span data-ttu-id="750c6-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="750c6-185">DateTimeOffset</span></span>    | <span data-ttu-id="750c6-p107">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="750c6-188">parentReference</span><span class="sxs-lookup"><span data-stu-id="750c6-188">parentReference</span></span>      | <span data-ttu-id="750c6-189">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="750c6-189">[itemReference][]</span></span> | <span data-ttu-id="750c6-p108">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="750c6-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="750c6-192">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="750c6-192">sharepointIds</span></span>        | <span data-ttu-id="750c6-193">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="750c6-193">[sharepointIds][]</span></span> | <span data-ttu-id="750c6-p109">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="750c6-196">webUrl</span><span class="sxs-lookup"><span data-stu-id="750c6-196">webUrl</span></span>               | <span data-ttu-id="750c6-197">string (url)</span><span class="sxs-lookup"><span data-stu-id="750c6-197">string (url)</span></span>      | <span data-ttu-id="750c6-p110">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="750c6-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="750c6-200">Relações</span><span class="sxs-lookup"><span data-stu-id="750c6-200">Relationships</span></span>

 <span data-ttu-id="750c6-201">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="750c6-201">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="750c6-202">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="750c6-202">Relationship name</span></span> | <span data-ttu-id="750c6-203">Tipo</span><span class="sxs-lookup"><span data-stu-id="750c6-203">Type</span></span>                           | <span data-ttu-id="750c6-204">Descrição</span><span class="sxs-lookup"><span data-stu-id="750c6-204">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="750c6-205">activities</span><span class="sxs-lookup"><span data-stu-id="750c6-205">activities</span></span>        | <span data-ttu-id="750c6-206">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="750c6-206">[itemActivity][] collection</span></span>    | <span data-ttu-id="750c6-207">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="750c6-207">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="750c6-208">análise</span><span class="sxs-lookup"><span data-stu-id="750c6-208">analytics</span></span>         | <span data-ttu-id="750c6-209">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="750c6-209">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="750c6-210">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="750c6-210">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="750c6-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="750c6-211">driveItem</span></span>         | <span data-ttu-id="750c6-212">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="750c6-212">[driveItem][]</span></span>                  | <span data-ttu-id="750c6-213">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="750c6-213">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="750c6-214">campos</span><span class="sxs-lookup"><span data-stu-id="750c6-214">fields</span></span>            | <span data-ttu-id="750c6-215">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="750c6-215">[fieldValueSet][]</span></span>              | <span data-ttu-id="750c6-216">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="750c6-216">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="750c6-217">versões</span><span class="sxs-lookup"><span data-stu-id="750c6-217">versions</span></span>          | <span data-ttu-id="750c6-218">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="750c6-218">[listItemVersion][] collection</span></span> | <span data-ttu-id="750c6-219">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="750c6-219">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="750c6-231">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="750c6-231">JSON representation</span></span>

<span data-ttu-id="750c6-232">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="750c6-232">Here is a JSON representation of a **listItem** resource.</span></span>

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

