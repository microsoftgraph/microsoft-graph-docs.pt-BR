---
author: JeremyKelley
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
description: O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: 81589377d30b0e1e2c494ade1ba9b48d7803495e
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239020"
---
# <a name="drive-resource-type"></a><span data-ttu-id="56a17-103">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="56a17-103">Drive resource type</span></span>

<span data-ttu-id="56a17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56a17-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56a17-105">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="56a17-105">The drive resource is the top-level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="56a17-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="56a17-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56a17-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56a17-108">JSON representation</span></span>

<span data-ttu-id="56a17-109">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="56a17-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="56a17-110">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="56a17-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="56a17-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56a17-111">Properties</span></span>

| <span data-ttu-id="56a17-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56a17-112">Property</span></span>             | <span data-ttu-id="56a17-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="56a17-113">Type</span></span>                          | <span data-ttu-id="56a17-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="56a17-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="56a17-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="56a17-115">createdBy</span></span>            | <span data-ttu-id="56a17-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="56a17-116">[identitySet][]</span></span>               | <span data-ttu-id="56a17-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="56a17-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56a17-119">createdDateTime</span></span>      | <span data-ttu-id="56a17-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a17-120">dateTimeOffset</span></span>                | <span data-ttu-id="56a17-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="56a17-123">description</span><span class="sxs-lookup"><span data-stu-id="56a17-123">description</span></span>          | <span data-ttu-id="56a17-124">String</span><span class="sxs-lookup"><span data-stu-id="56a17-124">String</span></span>                        | <span data-ttu-id="56a17-125">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="56a17-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="56a17-126">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="56a17-126">Read-write.</span></span>
| <span data-ttu-id="56a17-127">driveType</span><span class="sxs-lookup"><span data-stu-id="56a17-127">driveType</span></span>            | <span data-ttu-id="56a17-128">String</span><span class="sxs-lookup"><span data-stu-id="56a17-128">String</span></span>                        | <span data-ttu-id="56a17-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="56a17-134">id</span><span class="sxs-lookup"><span data-stu-id="56a17-134">id</span></span>                   | <span data-ttu-id="56a17-135">String</span><span class="sxs-lookup"><span data-stu-id="56a17-135">String</span></span>                        | <span data-ttu-id="56a17-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="56a17-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="56a17-138">lastModifiedBy</span></span>       | <span data-ttu-id="56a17-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="56a17-139">[identitySet][]</span></span>               | <span data-ttu-id="56a17-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="56a17-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56a17-142">lastModifiedDateTime</span></span> | <span data-ttu-id="56a17-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56a17-143">dateTimeOffset</span></span>                | <span data-ttu-id="56a17-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="56a17-146">nome</span><span class="sxs-lookup"><span data-stu-id="56a17-146">name</span></span>                 | <span data-ttu-id="56a17-147">string</span><span class="sxs-lookup"><span data-stu-id="56a17-147">string</span></span>                        | <span data-ttu-id="56a17-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="56a17-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="56a17-150">owner</span><span class="sxs-lookup"><span data-stu-id="56a17-150">owner</span></span>                | [<span data-ttu-id="56a17-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="56a17-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="56a17-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="56a17-155">quota</span><span class="sxs-lookup"><span data-stu-id="56a17-155">quota</span></span>                | [<span data-ttu-id="56a17-156">quota</span><span class="sxs-lookup"><span data-stu-id="56a17-156">quota</span></span>](quota.md)             | <span data-ttu-id="56a17-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="56a17-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="56a17-160">sharepointIds</span></span>        | <span data-ttu-id="56a17-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="56a17-161">[sharepointIds][]</span></span>             | <span data-ttu-id="56a17-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="56a17-164">sistema</span><span class="sxs-lookup"><span data-stu-id="56a17-164">system</span></span>               | <span data-ttu-id="56a17-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="56a17-165">[systemFacet][]</span></span>               | <span data-ttu-id="56a17-166">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="56a17-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="56a17-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-167">Read-only.</span></span>
| <span data-ttu-id="56a17-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="56a17-168">webUrl</span></span>               | <span data-ttu-id="56a17-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="56a17-169">string (url)</span></span>                  | <span data-ttu-id="56a17-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="56a17-175">Relações</span><span class="sxs-lookup"><span data-stu-id="56a17-175">Relationships</span></span>

| <span data-ttu-id="56a17-176">Relação</span><span class="sxs-lookup"><span data-stu-id="56a17-176">Relationship</span></span> | <span data-ttu-id="56a17-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="56a17-177">Type</span></span>                                 | <span data-ttu-id="56a17-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="56a17-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="56a17-179">following</span><span class="sxs-lookup"><span data-stu-id="56a17-179">following</span></span>    | <span data-ttu-id="56a17-180">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="56a17-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="56a17-181">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="56a17-181">The list of items the user is following.</span></span> <span data-ttu-id="56a17-182">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="56a17-182">Only in OneDrive for Business.</span></span>
| <span data-ttu-id="56a17-183">items</span><span class="sxs-lookup"><span data-stu-id="56a17-183">items</span></span>        | <span data-ttu-id="56a17-184">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="56a17-184">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="56a17-p116">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="56a17-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="56a17-188">root</span><span class="sxs-lookup"><span data-stu-id="56a17-188">root</span></span>         | [<span data-ttu-id="56a17-189">DriveItem</span><span class="sxs-lookup"><span data-stu-id="56a17-189">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="56a17-p117">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="56a17-192">special</span><span class="sxs-lookup"><span data-stu-id="56a17-192">special</span></span>      | <span data-ttu-id="56a17-193">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="56a17-193">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="56a17-194">Coleção de pastas comuns disponíveis no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="56a17-194">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="56a17-195">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-195">Read-only.</span></span> <span data-ttu-id="56a17-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="56a17-196">Nullable.</span></span>
| <span data-ttu-id="56a17-197">list</span><span class="sxs-lookup"><span data-stu-id="56a17-197">list</span></span>         | [<span data-ttu-id="56a17-198">List</span><span class="sxs-lookup"><span data-stu-id="56a17-198">List</span></span>](list.md)                      | <span data-ttu-id="56a17-199">Para unidades no SharePoint, a lista de biblioteca de documentos subjacentes.</span><span class="sxs-lookup"><span data-stu-id="56a17-199">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="56a17-200">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56a17-200">Read-only.</span></span> <span data-ttu-id="56a17-201">Anulável.</span><span class="sxs-lookup"><span data-stu-id="56a17-201">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="56a17-202">Métodos</span><span class="sxs-lookup"><span data-stu-id="56a17-202">Methods</span></span>

|                        <span data-ttu-id="56a17-203">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="56a17-203">Common task</span></span>                         |         <span data-ttu-id="56a17-204">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="56a17-204">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="56a17-205">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="56a17-205">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="56a17-206">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="56a17-206">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="56a17-207">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="56a17-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="56a17-208">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="56a17-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="56a17-209">[Listar os driveItems seguidos pelo usuário][drive-following]</span><span class="sxs-lookup"><span data-stu-id="56a17-209">[List user's followed driveItems][drive-following]</span></span>         | `Get /drive/following`       |
| <span data-ttu-id="56a17-210">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="56a17-210">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="56a17-211">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="56a17-211">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="56a17-212">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="56a17-212">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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

