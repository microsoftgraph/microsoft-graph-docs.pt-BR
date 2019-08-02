---
author: JeremyKelley
ms.author: JeremyKelley
title: tipo de recurso de unidade
description: o recurso de unidade representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 689c020a0c717fb395d13822c2c8de8f265988a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012720"
---
# <a name="drive-resource-type"></a><span data-ttu-id="493ec-103">tipo de recurso de unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-103">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="493ec-104">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="493ec-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="493ec-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="493ec-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="493ec-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="493ec-107">Methods</span></span>

|                        <span data-ttu-id="493ec-108">Método</span><span class="sxs-lookup"><span data-stu-id="493ec-108">Method</span></span>                              |         <span data-ttu-id="493ec-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="493ec-109">Return type</span></span>         | <span data-ttu-id="493ec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="493ec-110">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="493ec-111">[Obter unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="493ec-111">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="493ec-112">unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-112">drive</span></span>                       | <span data-ttu-id="493ec-113">Obter metadados sobre uma unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-113">Get metadata about a user's default drive on OneDrive.</span></span> |
| <span data-ttu-id="493ec-114">[Obter raiz da unidade][item-get]</span><span class="sxs-lookup"><span data-stu-id="493ec-114">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="493ec-115">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-115">[driveItem][]</span></span>               | <span data-ttu-id="493ec-116">Obter pasta raiz de uma unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-116">Get root folder for a drive</span></span> |
| <span data-ttu-id="493ec-117">[Listar atividades][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="493ec-117">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="493ec-118">Coleção de [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="493ec-118">[itemActivity][] collection</span></span> | <span data-ttu-id="493ec-119">Listar atividades que ocorreram na unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-119">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="493ec-120">[Listar itens seguidos][drive-following]</span><span class="sxs-lookup"><span data-stu-id="493ec-120">[List followed Items][drive-following]</span></span>                     | <span data-ttu-id="493ec-121">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-121">[driveItem][] collection</span></span>    | <span data-ttu-id="493ec-122">Listar os driveItems seguidos do usuário</span><span class="sxs-lookup"><span data-stu-id="493ec-122">List the user's followed driveItems</span></span> |
| <span data-ttu-id="493ec-123">[Listar secundários][item-children]</span><span class="sxs-lookup"><span data-stu-id="493ec-123">[List children][item-children]</span></span>                             | <span data-ttu-id="493ec-124">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-124">[driveItem][] collection</span></span>    | <span data-ttu-id="493ec-125">Listar secundários da pasta raiz de uma unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-125">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="493ec-126">[Listar alterações][item-changes]</span><span class="sxs-lookup"><span data-stu-id="493ec-126">[List changes][item-changes]</span></span>                               | <span data-ttu-id="493ec-127">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-127">[driveItem][] collection</span></span>    | <span data-ttu-id="493ec-128">Listar alterações de todos os driveItems na Unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-128">List changes for all Items in the Drive</span></span> |
| <span data-ttu-id="493ec-129">[Pesquisa][item-search]</span><span class="sxs-lookup"><span data-stu-id="493ec-129">[Search][item-search]</span></span>                                      | <span data-ttu-id="493ec-130">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-130">[driveItem][] collection</span></span>    | <span data-ttu-id="493ec-131">Pesquisar driveItems em uma unidade</span><span class="sxs-lookup"><span data-stu-id="493ec-131">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="493ec-132">Obter pasta especial</span><span class="sxs-lookup"><span data-stu-id="493ec-132">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="493ec-133">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-133">[driveItem][]</span></span>               | <span data-ttu-id="493ec-134">Acessar uma pasta especial por nome canônico</span><span class="sxs-lookup"><span data-stu-id="493ec-134">Access a special (named) folder in the user's OneDrive by its known name.</span></span> |


## <a name="properties"></a><span data-ttu-id="493ec-135">Propriedades</span><span class="sxs-lookup"><span data-stu-id="493ec-135">Properties</span></span>

| <span data-ttu-id="493ec-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="493ec-136">Property</span></span>             | <span data-ttu-id="493ec-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="493ec-137">Type</span></span>                          | <span data-ttu-id="493ec-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="493ec-138">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="493ec-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="493ec-139">createdBy</span></span>            | <span data-ttu-id="493ec-140">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="493ec-140">[identitySet][]</span></span>               | <span data-ttu-id="493ec-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="493ec-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="493ec-143">createdDateTime</span></span>      | <span data-ttu-id="493ec-144">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="493ec-144">dateTimeOffset</span></span>                | <span data-ttu-id="493ec-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="493ec-147">description</span><span class="sxs-lookup"><span data-stu-id="493ec-147">description</span></span>          | <span data-ttu-id="493ec-148">String</span><span class="sxs-lookup"><span data-stu-id="493ec-148">String</span></span>                        | <span data-ttu-id="493ec-149">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="493ec-149">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="493ec-150">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="493ec-150">Read-write.</span></span>
| <span data-ttu-id="493ec-151">driveType</span><span class="sxs-lookup"><span data-stu-id="493ec-151">driveType</span></span>            | <span data-ttu-id="493ec-152">String</span><span class="sxs-lookup"><span data-stu-id="493ec-152">String</span></span>                        | <span data-ttu-id="493ec-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="493ec-158">id</span><span class="sxs-lookup"><span data-stu-id="493ec-158">id</span></span>                   | <span data-ttu-id="493ec-159">String</span><span class="sxs-lookup"><span data-stu-id="493ec-159">String</span></span>                        | <span data-ttu-id="493ec-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="493ec-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="493ec-162">lastModifiedBy</span></span>       | <span data-ttu-id="493ec-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="493ec-163">[identitySet][]</span></span>               | <span data-ttu-id="493ec-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="493ec-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="493ec-166">lastModifiedDateTime</span></span> | <span data-ttu-id="493ec-167">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="493ec-167">dateTimeOffset</span></span>                | <span data-ttu-id="493ec-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="493ec-170">nome</span><span class="sxs-lookup"><span data-stu-id="493ec-170">name</span></span>                 | <span data-ttu-id="493ec-171">string</span><span class="sxs-lookup"><span data-stu-id="493ec-171">string</span></span>                        | <span data-ttu-id="493ec-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="493ec-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="493ec-174">owner</span><span class="sxs-lookup"><span data-stu-id="493ec-174">owner</span></span>                | [<span data-ttu-id="493ec-175">identitySet</span><span class="sxs-lookup"><span data-stu-id="493ec-175">identitySet</span></span>](identityset.md) | <span data-ttu-id="493ec-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="493ec-179">quota</span><span class="sxs-lookup"><span data-stu-id="493ec-179">quota</span></span>                | [<span data-ttu-id="493ec-180">quota</span><span class="sxs-lookup"><span data-stu-id="493ec-180">quota</span></span>](quota.md)             | <span data-ttu-id="493ec-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="493ec-184">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="493ec-184">sharepointIds</span></span>        | <span data-ttu-id="493ec-185">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="493ec-185">[sharepointIds][]</span></span>             | <span data-ttu-id="493ec-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="493ec-188">sistema</span><span class="sxs-lookup"><span data-stu-id="493ec-188">system</span></span>               | <span data-ttu-id="493ec-189">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="493ec-189">[systemFacet][]</span></span>               | <span data-ttu-id="493ec-190">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="493ec-190">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="493ec-191">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-191">Read-only.</span></span>
| <span data-ttu-id="493ec-192">webUrl</span><span class="sxs-lookup"><span data-stu-id="493ec-192">webUrl</span></span>               | <span data-ttu-id="493ec-193">string (url)</span><span class="sxs-lookup"><span data-stu-id="493ec-193">string (url)</span></span>                  | <span data-ttu-id="493ec-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="493ec-199">Relações</span><span class="sxs-lookup"><span data-stu-id="493ec-199">Relationships</span></span>

| <span data-ttu-id="493ec-200">Relação</span><span class="sxs-lookup"><span data-stu-id="493ec-200">Relationship</span></span> | <span data-ttu-id="493ec-201">Tipo</span><span class="sxs-lookup"><span data-stu-id="493ec-201">Type</span></span>                                 | <span data-ttu-id="493ec-202">Descrição</span><span class="sxs-lookup"><span data-stu-id="493ec-202">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="493ec-203">activities</span><span class="sxs-lookup"><span data-stu-id="493ec-203">activities</span></span>   | <span data-ttu-id="493ec-204">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="493ec-204">[itemActivity][] collection</span></span>          | <span data-ttu-id="493ec-205">A lista de atividades recentes que ocorreram nesta unidade.</span><span class="sxs-lookup"><span data-stu-id="493ec-205">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="493ec-206">pacotes</span><span class="sxs-lookup"><span data-stu-id="493ec-206">Multiple bundles</span></span>      | <span data-ttu-id="493ec-207">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-207">[driveItem][] collection</span></span>             | <span data-ttu-id="493ec-208">Coleção de [pacotes][bundle] (álbuns e conjuntos de itens compartilhados com seleção múltipla).</span><span class="sxs-lookup"><span data-stu-id="493ec-208">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="493ec-209">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="493ec-209">Only in personal OneDrive.</span></span>
| <span data-ttu-id="493ec-210">following</span><span class="sxs-lookup"><span data-stu-id="493ec-210">following</span></span>    | <span data-ttu-id="493ec-211">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-211">[driveItem][] collection</span></span>             | <span data-ttu-id="493ec-212">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="493ec-212">The list of items the user is following.</span></span> <span data-ttu-id="493ec-213">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="493ec-213">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="493ec-214">items</span><span class="sxs-lookup"><span data-stu-id="493ec-214">items</span></span>        | <span data-ttu-id="493ec-215">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-215">[driveItem][] collection</span></span>             | <span data-ttu-id="493ec-p117">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="493ec-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="493ec-219">root</span><span class="sxs-lookup"><span data-stu-id="493ec-219">root</span></span>         | <span data-ttu-id="493ec-220">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-220">[driveItem][]</span></span>                        | <span data-ttu-id="493ec-p118">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="493ec-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="493ec-223">special</span><span class="sxs-lookup"><span data-stu-id="493ec-223">special</span></span>      | <span data-ttu-id="493ec-224">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="493ec-224">[driveItem][] collection</span></span>             | <span data-ttu-id="493ec-p119">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="493ec-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="493ec-228">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="493ec-228">JSON representation</span></span>

<span data-ttu-id="493ec-229">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="493ec-229">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="493ec-230">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="493ec-230">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "activities",
    "createdBy",
    "createdDateTime",
    "description",
    "lastModifiedBy",
    "lastModifiedDateTime",
    "name",
    "webUrl",
    "items",
    "root",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "id": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [{"@odata.type": "microsoft.graph.driveItem"}],
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.identitySet"},
  "quota": {"@odata.type": "microsoft.graph.quota"},
  "root": {"@odata.type": "microsoft.graph.driveItem"},
  "special": [{"@odata.type": "microsoft.graph.driveItem"}],
  "system": {"@odata.type": "microsoft.graph.systemFacet"},
  "webUrl": "string",
  "sharepointIds": {"@odata.type": "microsoft.graph.sharepointIds"}
}
```


[bundle]: bundle.md
[driveItem]: driveItem.md
[itemActivity]: itemactivity.md
[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-activities]: ../api/activities-list.md
[drive-following]: ../api/drive-list-following.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": {
    "Resources/Drive": "#"
  },
  "suppressions": []
}
-->
