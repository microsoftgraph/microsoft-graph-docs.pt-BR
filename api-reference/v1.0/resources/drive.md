---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
description: O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: c389d801f8aea070dd310e1d826c9139298578cd
ms.sourcegitcommit: eafb1629e52450dab0da6a1fb6d1ddfa878777c6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2020
ms.locfileid: "49082283"
---
# <a name="drive-resource-type"></a><span data-ttu-id="b02b4-103">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="b02b4-103">Drive resource type</span></span>

<span data-ttu-id="b02b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b02b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b02b4-105">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b02b4-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="b02b4-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b02b4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b02b4-108">JSON representation</span></span>

<span data-ttu-id="b02b4-109">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="b02b4-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="b02b4-110">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="b02b4-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
    "sharepointIds",
    "special",
    "system"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.drive"
}-->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [{"@odata.type": "microsoft.graph.driveItem"}],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b02b4-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b02b4-111">Properties</span></span>

| <span data-ttu-id="b02b4-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b02b4-112">Property</span></span>             | <span data-ttu-id="b02b4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b02b4-113">Type</span></span>                          | <span data-ttu-id="b02b4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b02b4-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b02b4-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="b02b4-115">createdBy</span></span>            | <span data-ttu-id="b02b4-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b02b4-116">[identitySet][]</span></span>               | <span data-ttu-id="b02b4-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="b02b4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b02b4-119">createdDateTime</span></span>      | <span data-ttu-id="b02b4-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b02b4-120">dateTimeOffset</span></span>                | <span data-ttu-id="b02b4-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="b02b4-123">description</span><span class="sxs-lookup"><span data-stu-id="b02b4-123">description</span></span>          | <span data-ttu-id="b02b4-124">String</span><span class="sxs-lookup"><span data-stu-id="b02b4-124">String</span></span>                        | <span data-ttu-id="b02b4-125">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="b02b4-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="b02b4-126">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="b02b4-126">Read-write.</span></span>
| <span data-ttu-id="b02b4-127">driveType</span><span class="sxs-lookup"><span data-stu-id="b02b4-127">driveType</span></span>            | <span data-ttu-id="b02b4-128">String</span><span class="sxs-lookup"><span data-stu-id="b02b4-128">String</span></span>                        | <span data-ttu-id="b02b4-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="b02b4-134">id</span><span class="sxs-lookup"><span data-stu-id="b02b4-134">id</span></span>                   | <span data-ttu-id="b02b4-135">String</span><span class="sxs-lookup"><span data-stu-id="b02b4-135">String</span></span>                        | <span data-ttu-id="b02b4-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="b02b4-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b02b4-138">lastModifiedBy</span></span>       | <span data-ttu-id="b02b4-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b02b4-139">[identitySet][]</span></span>               | <span data-ttu-id="b02b4-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="b02b4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b02b4-142">lastModifiedDateTime</span></span> | <span data-ttu-id="b02b4-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b02b4-143">dateTimeOffset</span></span>                | <span data-ttu-id="b02b4-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="b02b4-146">nome</span><span class="sxs-lookup"><span data-stu-id="b02b4-146">name</span></span>                 | <span data-ttu-id="b02b4-147">string</span><span class="sxs-lookup"><span data-stu-id="b02b4-147">string</span></span>                        | <span data-ttu-id="b02b4-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="b02b4-150">owner</span><span class="sxs-lookup"><span data-stu-id="b02b4-150">owner</span></span>                | [<span data-ttu-id="b02b4-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="b02b4-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="b02b4-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="b02b4-155">quota</span><span class="sxs-lookup"><span data-stu-id="b02b4-155">quota</span></span>                | [<span data-ttu-id="b02b4-156">quota</span><span class="sxs-lookup"><span data-stu-id="b02b4-156">quota</span></span>](quota.md)             | <span data-ttu-id="b02b4-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="b02b4-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b02b4-160">sharepointIds</span></span>        | <span data-ttu-id="b02b4-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b02b4-161">[sharepointIds][]</span></span>             | <span data-ttu-id="b02b4-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="b02b4-164">sistema</span><span class="sxs-lookup"><span data-stu-id="b02b4-164">system</span></span>               | <span data-ttu-id="b02b4-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="b02b4-165">[systemFacet][]</span></span>               | <span data-ttu-id="b02b4-166">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="b02b4-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="b02b4-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-167">Read-only.</span></span>
| <span data-ttu-id="b02b4-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="b02b4-168">webUrl</span></span>               | <span data-ttu-id="b02b4-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="b02b4-169">string (url)</span></span>                  | <span data-ttu-id="b02b4-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="b02b4-175">Relações</span><span class="sxs-lookup"><span data-stu-id="b02b4-175">Relationships</span></span>

| <span data-ttu-id="b02b4-176">Relação</span><span class="sxs-lookup"><span data-stu-id="b02b4-176">Relationship</span></span> | <span data-ttu-id="b02b4-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="b02b4-177">Type</span></span>                                 | <span data-ttu-id="b02b4-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="b02b4-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="b02b4-179">following</span><span class="sxs-lookup"><span data-stu-id="b02b4-179">following</span></span>    | <span data-ttu-id="b02b4-180">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b02b4-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="b02b4-181">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="b02b4-181">The list of items the user is following.</span></span> <span data-ttu-id="b02b4-182">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b02b4-182">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="b02b4-183">items</span><span class="sxs-lookup"><span data-stu-id="b02b4-183">items</span></span>        | <span data-ttu-id="b02b4-184">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b02b4-184">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="b02b4-p116">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="b02b4-188">root</span><span class="sxs-lookup"><span data-stu-id="b02b4-188">root</span></span>         | [<span data-ttu-id="b02b4-189">DriveItem</span><span class="sxs-lookup"><span data-stu-id="b02b4-189">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="b02b4-p117">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="b02b4-192">special</span><span class="sxs-lookup"><span data-stu-id="b02b4-192">special</span></span>      | <span data-ttu-id="b02b4-193">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="b02b4-193">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="b02b4-194">Coleção de pastas comuns disponíveis no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b02b4-194">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="b02b4-195">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-195">Read-only.</span></span> <span data-ttu-id="b02b4-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b02b4-196">Nullable.</span></span>
| <span data-ttu-id="b02b4-197">list</span><span class="sxs-lookup"><span data-stu-id="b02b4-197">list</span></span>         | [<span data-ttu-id="b02b4-198">List</span><span class="sxs-lookup"><span data-stu-id="b02b4-198">List</span></span>](list.md)                      | <span data-ttu-id="b02b4-199">Para unidades no SharePoint, a lista de biblioteca de documentos subjacentes.</span><span class="sxs-lookup"><span data-stu-id="b02b4-199">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="b02b4-200">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b02b4-200">Read-only.</span></span> <span data-ttu-id="b02b4-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="b02b4-201">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="b02b4-202">Métodos</span><span class="sxs-lookup"><span data-stu-id="b02b4-202">Methods</span></span>

|                        <span data-ttu-id="b02b4-203">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="b02b4-203">Common task</span></span>                         |         <span data-ttu-id="b02b4-204">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="b02b4-204">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="b02b4-205">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="b02b4-205">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="b02b4-206">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="b02b4-206">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="b02b4-207">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="b02b4-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="b02b4-208">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="b02b4-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="b02b4-209">[Listar os driveItems seguidos pelo usuário][drive-following]</span><span class="sxs-lookup"><span data-stu-id="b02b4-209">[List user's followed driveItems][drive-following]</span></span>         | `Get /drive/following`       |
| <span data-ttu-id="b02b4-210">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="b02b4-210">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="b02b4-211">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="b02b4-211">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="b02b4-212">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="b02b4-212">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md
[drive-following]: ../api/drive-list-following.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/drive.md:
      Found potential enums in resource example that weren't defined in a table:(personal,business,documentLibrary) are in resource, but () are in table"
  ],
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->

