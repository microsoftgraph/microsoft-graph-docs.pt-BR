---
author: JeremyKelley
ms.author: JeremyKelley
title: tipo de recurso de unidade
description: o recurso de unidade representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 74ef4a5f8c2e67a81ad02ca0844d7f15dba972e8
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49081828"
---
# <a name="drive-resource-type"></a><span data-ttu-id="c9888-103">tipo de recurso de unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-103">drive resource type</span></span>

<span data-ttu-id="c9888-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9888-105">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c9888-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="c9888-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="c9888-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="methods"></a><span data-ttu-id="c9888-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c9888-108">Methods</span></span>

|                        <span data-ttu-id="c9888-109">Método</span><span class="sxs-lookup"><span data-stu-id="c9888-109">Method</span></span>                              |         <span data-ttu-id="c9888-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c9888-110">Return type</span></span>         | <span data-ttu-id="c9888-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9888-111">Description</span></span> |
| :--------------------------------------------------------- | :-------------------------- |-------------|
| <span data-ttu-id="c9888-112">[Obter unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="c9888-112">[Get drive][drive-get]</span></span>                                     | <span data-ttu-id="c9888-113">unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-113">drive</span></span>                       | <span data-ttu-id="c9888-114">Obter metadados sobre uma unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-114">Get metadata about a drive</span></span> |
| <span data-ttu-id="c9888-115">[Obter raiz da unidade][item-get]</span><span class="sxs-lookup"><span data-stu-id="c9888-115">[Get drive root][item-get]</span></span>                                 | <span data-ttu-id="c9888-116">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-116">[driveItem][]</span></span>               | <span data-ttu-id="c9888-117">Obter pasta raiz de uma unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-117">Get root folder of a drive</span></span> |
| <span data-ttu-id="c9888-118">[Listar atividades][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="c9888-118">[List activities][drive-activities]</span></span>                        | <span data-ttu-id="c9888-119">Coleção de [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="c9888-119">[itemActivity][] collection</span></span> | <span data-ttu-id="c9888-120">Listar atividades que ocorreram na unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-120">List activities that occurred under the drive</span></span> |
| <span data-ttu-id="c9888-121">[Listar itens seguidos][drive-following]</span><span class="sxs-lookup"><span data-stu-id="c9888-121">[List followed items][drive-following]</span></span>                     | <span data-ttu-id="c9888-122">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-122">[driveItem][] collection</span></span>    | <span data-ttu-id="c9888-123">Listar os driveItems seguidos do usuário</span><span class="sxs-lookup"><span data-stu-id="c9888-123">List the user's followed driveItems</span></span> |
| <span data-ttu-id="c9888-124">[Listar secundários][item-children]</span><span class="sxs-lookup"><span data-stu-id="c9888-124">[List children][item-children]</span></span>                             | <span data-ttu-id="c9888-125">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-125">[driveItem][] collection</span></span>    | <span data-ttu-id="c9888-126">Listar secundários da pasta raiz de uma unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-126">List children of the root folder of a drive</span></span> |
| <span data-ttu-id="c9888-127">[Listar alterações][item-changes]</span><span class="sxs-lookup"><span data-stu-id="c9888-127">[List changes][item-changes]</span></span>                               | <span data-ttu-id="c9888-128">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-128">[driveItem][] collection</span></span>    | <span data-ttu-id="c9888-129">Listar alterações de todos os driveItems na Unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-129">List changes for all driveItems in the Drive</span></span> |
| <span data-ttu-id="c9888-130">[Pesquisa][item-search]</span><span class="sxs-lookup"><span data-stu-id="c9888-130">[Search][item-search]</span></span>                                      | <span data-ttu-id="c9888-131">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-131">[driveItem][] collection</span></span>    | <span data-ttu-id="c9888-132">Pesquisar driveItems em uma unidade</span><span class="sxs-lookup"><span data-stu-id="c9888-132">Search for driveItems in a drive</span></span> |
| [<span data-ttu-id="c9888-133">Obter pasta especial</span><span class="sxs-lookup"><span data-stu-id="c9888-133">Get special folder</span></span>](../api/drive-get-specialfolder.md)    | <span data-ttu-id="c9888-134">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-134">[driveItem][]</span></span>               | <span data-ttu-id="c9888-135">Acessar uma pasta especial por nome canônico</span><span class="sxs-lookup"><span data-stu-id="c9888-135">Access a special folder by its canonical name</span></span> |


## <a name="properties"></a><span data-ttu-id="c9888-136">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9888-136">Properties</span></span>

| <span data-ttu-id="c9888-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9888-137">Property</span></span>             | <span data-ttu-id="c9888-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9888-138">Type</span></span>                          | <span data-ttu-id="c9888-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9888-139">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="c9888-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="c9888-140">createdBy</span></span>            | <span data-ttu-id="c9888-141">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c9888-141">[identitySet][]</span></span>               | <span data-ttu-id="c9888-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="c9888-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9888-144">createdDateTime</span></span>      | <span data-ttu-id="c9888-145">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9888-145">dateTimeOffset</span></span>                | <span data-ttu-id="c9888-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="c9888-148">description</span><span class="sxs-lookup"><span data-stu-id="c9888-148">description</span></span>          | <span data-ttu-id="c9888-149">String</span><span class="sxs-lookup"><span data-stu-id="c9888-149">String</span></span>                        | <span data-ttu-id="c9888-150">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="c9888-150">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="c9888-151">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="c9888-151">Read-write.</span></span>
| <span data-ttu-id="c9888-152">driveType</span><span class="sxs-lookup"><span data-stu-id="c9888-152">driveType</span></span>            | <span data-ttu-id="c9888-153">String</span><span class="sxs-lookup"><span data-stu-id="c9888-153">String</span></span>                        | <span data-ttu-id="c9888-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="c9888-159">id</span><span class="sxs-lookup"><span data-stu-id="c9888-159">id</span></span>                   | <span data-ttu-id="c9888-160">String</span><span class="sxs-lookup"><span data-stu-id="c9888-160">String</span></span>                        | <span data-ttu-id="c9888-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="c9888-163">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c9888-163">lastModifiedBy</span></span>       | <span data-ttu-id="c9888-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c9888-164">[identitySet][]</span></span>               | <span data-ttu-id="c9888-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="c9888-167">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9888-167">lastModifiedDateTime</span></span> | <span data-ttu-id="c9888-168">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9888-168">dateTimeOffset</span></span>                | <span data-ttu-id="c9888-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="c9888-171">nome</span><span class="sxs-lookup"><span data-stu-id="c9888-171">name</span></span>                 | <span data-ttu-id="c9888-172">string</span><span class="sxs-lookup"><span data-stu-id="c9888-172">string</span></span>                        | <span data-ttu-id="c9888-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="c9888-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="c9888-175">owner</span><span class="sxs-lookup"><span data-stu-id="c9888-175">owner</span></span>                | [<span data-ttu-id="c9888-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="c9888-176">identitySet</span></span>](identityset.md) | <span data-ttu-id="c9888-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="c9888-180">quota</span><span class="sxs-lookup"><span data-stu-id="c9888-180">quota</span></span>                | [<span data-ttu-id="c9888-181">quota</span><span class="sxs-lookup"><span data-stu-id="c9888-181">quota</span></span>](quota.md)             | <span data-ttu-id="c9888-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="c9888-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="c9888-185">sharepointIds</span></span>        | <span data-ttu-id="c9888-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="c9888-186">[sharepointIds][]</span></span>             | <span data-ttu-id="c9888-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="c9888-189">sistema</span><span class="sxs-lookup"><span data-stu-id="c9888-189">system</span></span>               | <span data-ttu-id="c9888-190">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="c9888-190">[systemFacet][]</span></span>               | <span data-ttu-id="c9888-191">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="c9888-191">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="c9888-192">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-192">Read-only.</span></span>
| <span data-ttu-id="c9888-193">webUrl</span><span class="sxs-lookup"><span data-stu-id="c9888-193">webUrl</span></span>               | <span data-ttu-id="c9888-194">string (url)</span><span class="sxs-lookup"><span data-stu-id="c9888-194">string (url)</span></span>                  | <span data-ttu-id="c9888-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="c9888-200">Relações</span><span class="sxs-lookup"><span data-stu-id="c9888-200">Relationships</span></span>

| <span data-ttu-id="c9888-201">Relação</span><span class="sxs-lookup"><span data-stu-id="c9888-201">Relationship</span></span> | <span data-ttu-id="c9888-202">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9888-202">Type</span></span>                                 | <span data-ttu-id="c9888-203">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9888-203">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="c9888-204">activities</span><span class="sxs-lookup"><span data-stu-id="c9888-204">activities</span></span>   | <span data-ttu-id="c9888-205">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="c9888-205">[itemActivity][] collection</span></span>          | <span data-ttu-id="c9888-206">A lista de atividades recentes que ocorreram nesta unidade.</span><span class="sxs-lookup"><span data-stu-id="c9888-206">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="c9888-207">pacotes</span><span class="sxs-lookup"><span data-stu-id="c9888-207">bundles</span></span>      | <span data-ttu-id="c9888-208">Coleção de [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-208">[driveItem][] collection</span></span>             | <span data-ttu-id="c9888-209">Coleção de [pacotes][bundle] (álbuns e conjuntos de itens compartilhados com seleção múltipla).</span><span class="sxs-lookup"><span data-stu-id="c9888-209">Collection of [bundles][bundle] (albums and multi-select-shared sets of items).</span></span> <span data-ttu-id="c9888-210">Somente no OneDrive pessoal.</span><span class="sxs-lookup"><span data-stu-id="c9888-210">Only in personal OneDrive.</span></span>
| <span data-ttu-id="c9888-211">following</span><span class="sxs-lookup"><span data-stu-id="c9888-211">following</span></span>    | <span data-ttu-id="c9888-212">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-212">[driveItem][] collection</span></span>             | <span data-ttu-id="c9888-213">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="c9888-213">The list of items the user is following.</span></span> <span data-ttu-id="c9888-214">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c9888-214">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="c9888-215">items</span><span class="sxs-lookup"><span data-stu-id="c9888-215">items</span></span>        | <span data-ttu-id="c9888-216">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-216">[driveItem][] collection</span></span>             | <span data-ttu-id="c9888-p117">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9888-p117">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="c9888-220">root</span><span class="sxs-lookup"><span data-stu-id="c9888-220">root</span></span>         | <span data-ttu-id="c9888-221">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-221">[driveItem][]</span></span>                        | <span data-ttu-id="c9888-p118">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c9888-p118">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="c9888-224">special</span><span class="sxs-lookup"><span data-stu-id="c9888-224">special</span></span>      | <span data-ttu-id="c9888-225">Coleção [driveItem][]</span><span class="sxs-lookup"><span data-stu-id="c9888-225">[driveItem][] collection</span></span>             | <span data-ttu-id="c9888-p119">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="c9888-p119">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c9888-229">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9888-229">JSON representation</span></span>

<span data-ttu-id="c9888-230">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="c9888-230">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="c9888-231">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="c9888-231">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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


