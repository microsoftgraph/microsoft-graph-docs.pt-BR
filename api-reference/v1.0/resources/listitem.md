---
author: JeremyKelley
ms.author: JeremyKelley
title: recurso listItem
description: Representa um item em uma lista do sharepoint.
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96c61daea047f969f88352429a46fc7efb8b776d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447560"
---
# <a name="listitem-resource"></a><span data-ttu-id="3239e-103">recurso listItem</span><span class="sxs-lookup"><span data-stu-id="3239e-103">listItem resource</span></span>

<span data-ttu-id="3239e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3239e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3239e-105">Representa um item em uma **[lista][]** do Sharepoint.</span><span class="sxs-lookup"><span data-stu-id="3239e-105">Represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="3239e-106">Os valores de coluna na lista estão disponíveis por meio do dicionário `fieldValueSet`.</span><span class="sxs-lookup"><span data-stu-id="3239e-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="3239e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3239e-107">Methods</span></span>

<span data-ttu-id="3239e-108">Os métodos a seguir estão disponíveis para recursos **listItem**.</span><span class="sxs-lookup"><span data-stu-id="3239e-108">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="3239e-109">Todos os exemplos são relativos a uma **[lista][]**:`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span><span class="sxs-lookup"><span data-stu-id="3239e-109">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="3239e-110">Método</span><span class="sxs-lookup"><span data-stu-id="3239e-110">Method</span></span>                    | <span data-ttu-id="3239e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3239e-111">Return Type</span></span> | <span data-ttu-id="3239e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3239e-112">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="3239e-113">[Get][]</span><span class="sxs-lookup"><span data-stu-id="3239e-113">[Get][]</span></span>                   | <span data-ttu-id="3239e-114">listItem</span><span class="sxs-lookup"><span data-stu-id="3239e-114">listItem</span></span>| <span data-ttu-id="3239e-115">Obter um item em uma lista.</span><span class="sxs-lookup"><span data-stu-id="3239e-115">Get an item in a list.</span></span>
| <span data-ttu-id="3239e-116">[Obter valores de coluna][Obter]</span><span class="sxs-lookup"><span data-stu-id="3239e-116">[Get column values][Get]</span></span>       | <span data-ttu-id="3239e-117">listItem</span><span class="sxs-lookup"><span data-stu-id="3239e-117">listItem</span></span> | <span data-ttu-id="3239e-118">Obter valores de coluna de listItem.</span><span class="sxs-lookup"><span data-stu-id="3239e-118">Get column values from listItem.</span></span>
| <span data-ttu-id="3239e-119">[Obter análises][]</span><span class="sxs-lookup"><span data-stu-id="3239e-119">[Get analytics][]</span></span>              | <span data-ttu-id="3239e-120">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="3239e-120">[itemAnalytics][]</span></span>| <span data-ttu-id="3239e-121">Obter análises para este recurso.</span><span class="sxs-lookup"><span data-stu-id="3239e-121">Get analytics for this resource.</span></span> 
| <span data-ttu-id="3239e-122">[Obter atividades por intervalo][]</span><span class="sxs-lookup"><span data-stu-id="3239e-122">[Get activities by interval][]</span></span> | <span data-ttu-id="3239e-123">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="3239e-123">[itemActivityStat][]</span></span>| <span data-ttu-id="3239e-124">Obter uma coleção de itemActivityStats dentro do intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="3239e-124">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="3239e-125">[Criar][]</span><span class="sxs-lookup"><span data-stu-id="3239e-125">[Create][]</span></span>                     | <span data-ttu-id="3239e-126">listItem</span><span class="sxs-lookup"><span data-stu-id="3239e-126">listItem</span></span> | <span data-ttu-id="3239e-127">Criar um novo listItem em uma lista.</span><span class="sxs-lookup"><span data-stu-id="3239e-127">Create a new listItem in a list.</span></span>
| <span data-ttu-id="3239e-128">[Excluir][]</span><span class="sxs-lookup"><span data-stu-id="3239e-128">[Delete][]</span></span>                     | <span data-ttu-id="3239e-129">Sem Conteúdo</span><span class="sxs-lookup"><span data-stu-id="3239e-129">No Content</span></span> | <span data-ttu-id="3239e-130">Remove um item de uma lista.</span><span class="sxs-lookup"><span data-stu-id="3239e-130">Removes an item from a list.</span></span>
| <span data-ttu-id="3239e-131">[Atualizar][]</span><span class="sxs-lookup"><span data-stu-id="3239e-131">[Update][]</span></span>                     | <span data-ttu-id="3239e-132">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="3239e-132">[fieldValueSet][]</span></span>| <span data-ttu-id="3239e-133">Atualizar as propriedades de um listItem.</span><span class="sxs-lookup"><span data-stu-id="3239e-133">Update the properties on a listItem.</span></span>
| <span data-ttu-id="3239e-134">[Atualizar valores de coluna][Atualizar]</span><span class="sxs-lookup"><span data-stu-id="3239e-134">[Update column values][Update]</span></span> | <span data-ttu-id="3239e-135">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="3239e-135">[fieldValueSet][]</span></span>| <span data-ttu-id="3239e-136">Atualizar os valores de coluna de um listItem.</span><span class="sxs-lookup"><span data-stu-id="3239e-136">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3239e-145">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3239e-145">Properties</span></span>

<span data-ttu-id="3239e-146">O recurso **listItem** tem as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="3239e-146">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="3239e-147">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3239e-147">Property name</span></span> | <span data-ttu-id="3239e-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="3239e-148">Type</span></span>                | <span data-ttu-id="3239e-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="3239e-149">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="3239e-150">contentType</span><span class="sxs-lookup"><span data-stu-id="3239e-150">contentType</span></span>   | <span data-ttu-id="3239e-151">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="3239e-151">[contentTypeInfo][]</span></span> | <span data-ttu-id="3239e-152">O tipo de conteúdo deste item de lista</span><span class="sxs-lookup"><span data-stu-id="3239e-152">The content type of this list item</span></span>

<span data-ttu-id="3239e-153">As propriedades a seguir são herdadas do **[baseItem][]**.</span><span class="sxs-lookup"><span data-stu-id="3239e-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="3239e-154">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="3239e-154">Property name</span></span>        | <span data-ttu-id="3239e-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="3239e-155">Type</span></span>              | <span data-ttu-id="3239e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="3239e-156">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="3239e-157">id</span><span class="sxs-lookup"><span data-stu-id="3239e-157">id</span></span>                   | <span data-ttu-id="3239e-158">string</span><span class="sxs-lookup"><span data-stu-id="3239e-158">string</span></span>            | <span data-ttu-id="3239e-p103">O identificador exclusivo do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="3239e-161">name</span><span class="sxs-lookup"><span data-stu-id="3239e-161">name</span></span>                 | <span data-ttu-id="3239e-162">string</span><span class="sxs-lookup"><span data-stu-id="3239e-162">string</span></span>            | <span data-ttu-id="3239e-163">O nome/título do item.</span><span class="sxs-lookup"><span data-stu-id="3239e-163">The name / title of the item.</span></span>
| <span data-ttu-id="3239e-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="3239e-164">createdBy</span></span>            | <span data-ttu-id="3239e-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3239e-165">[identitySet][]</span></span>   | <span data-ttu-id="3239e-166">Identidade do criador desse item.</span><span class="sxs-lookup"><span data-stu-id="3239e-166">Identity of the creator of this item.</span></span> <span data-ttu-id="3239e-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-167">Read-only.</span></span>
| <span data-ttu-id="3239e-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3239e-168">createdDateTime</span></span>      | <span data-ttu-id="3239e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3239e-169">DateTimeOffset</span></span>    | <span data-ttu-id="3239e-p105">A data e a hora da criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="3239e-172">description</span><span class="sxs-lookup"><span data-stu-id="3239e-172">description</span></span>          | <span data-ttu-id="3239e-173">string</span><span class="sxs-lookup"><span data-stu-id="3239e-173">string</span></span>            | <span data-ttu-id="3239e-174">O texto descritivo do item.</span><span class="sxs-lookup"><span data-stu-id="3239e-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="3239e-175">eTag</span><span class="sxs-lookup"><span data-stu-id="3239e-175">eTag</span></span>                 | <span data-ttu-id="3239e-176">string</span><span class="sxs-lookup"><span data-stu-id="3239e-176">string</span></span>            | <span data-ttu-id="3239e-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="3239e-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3239e-179">lastModifiedBy</span></span>       | <span data-ttu-id="3239e-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3239e-180">[identitySet][]</span></span>   | <span data-ttu-id="3239e-181">Identidade da última pessoa que alterou esse item.</span><span class="sxs-lookup"><span data-stu-id="3239e-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="3239e-182">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-182">Read-only.</span></span>
| <span data-ttu-id="3239e-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3239e-183">lastModifiedDateTime</span></span> | <span data-ttu-id="3239e-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3239e-184">DateTimeOffset</span></span>    | <span data-ttu-id="3239e-p108">A data e a hora que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="3239e-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="3239e-187">parentReference</span></span>      | <span data-ttu-id="3239e-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3239e-188">[itemReference][]</span></span> | <span data-ttu-id="3239e-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="3239e-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="3239e-191">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="3239e-191">sharepointIds</span></span>        | <span data-ttu-id="3239e-192">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="3239e-192">[sharepointIds][]</span></span> | <span data-ttu-id="3239e-p110">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="3239e-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="3239e-195">webUrl</span></span>               | <span data-ttu-id="3239e-196">string (url)</span><span class="sxs-lookup"><span data-stu-id="3239e-196">string (url)</span></span>      | <span data-ttu-id="3239e-p111">A URL que exibe o item no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3239e-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="3239e-199">Relações</span><span class="sxs-lookup"><span data-stu-id="3239e-199">Relationships</span></span>

 <span data-ttu-id="3239e-200">O recurso **listItem** tem as seguintes relações com outros recursos.</span><span class="sxs-lookup"><span data-stu-id="3239e-200">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="3239e-201">Nome da relação</span><span class="sxs-lookup"><span data-stu-id="3239e-201">Relationship name</span></span> | <span data-ttu-id="3239e-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="3239e-202">Type</span></span>                           | <span data-ttu-id="3239e-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="3239e-203">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="3239e-204">activities</span><span class="sxs-lookup"><span data-stu-id="3239e-204">activities</span></span>        | <span data-ttu-id="3239e-205">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="3239e-205">[itemActivity][] collection</span></span>    | <span data-ttu-id="3239e-206">A lista de atividades recentes que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="3239e-206">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="3239e-207">análise</span><span class="sxs-lookup"><span data-stu-id="3239e-207">analytics</span></span>         | <span data-ttu-id="3239e-208">recurso [itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="3239e-208">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="3239e-209">Análise sobre as atividades de visualização que ocorreram neste item.</span><span class="sxs-lookup"><span data-stu-id="3239e-209">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="3239e-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="3239e-210">driveItem</span></span>         | <span data-ttu-id="3239e-211">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="3239e-211">[driveItem][]</span></span>                  | <span data-ttu-id="3239e-212">Para bibliotecas de documentos, a relação **driveItem** expõe listItem como um **[driveItem][]**</span><span class="sxs-lookup"><span data-stu-id="3239e-212">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="3239e-213">campos</span><span class="sxs-lookup"><span data-stu-id="3239e-213">fields</span></span>            | <span data-ttu-id="3239e-214">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="3239e-214">[fieldValueSet][]</span></span>              | <span data-ttu-id="3239e-215">Os valores das colunas definidos neste item de lista.</span><span class="sxs-lookup"><span data-stu-id="3239e-215">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="3239e-216">versões</span><span class="sxs-lookup"><span data-stu-id="3239e-216">versions</span></span>          | <span data-ttu-id="3239e-217">coleção [listItemVersion][] </span><span class="sxs-lookup"><span data-stu-id="3239e-217">[listItemVersion][] collection</span></span> | <span data-ttu-id="3239e-218">A lista de versões anteriores do item de lista.</span><span class="sxs-lookup"><span data-stu-id="3239e-218">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="3239e-230">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3239e-230">JSON representation</span></span>

<span data-ttu-id="3239e-231">Veja a seguir uma representação JSON de um recurso **listItem**.</span><span class="sxs-lookup"><span data-stu-id="3239e-231">Here is a JSON representation of a **listItem** resource.</span></span>

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
