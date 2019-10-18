---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
description: O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: ba40d2ac0605a255b0b7df05db1e5bebb68c2e42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030538"
---
# <a name="drive-resource-type"></a><span data-ttu-id="1b234-103">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="1b234-103">Drive resource type</span></span>

<span data-ttu-id="1b234-104">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="1b234-104">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="1b234-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="1b234-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b234-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b234-107">JSON representation</span></span>

<span data-ttu-id="1b234-108">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="1b234-108">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="1b234-109">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="1b234-109">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1b234-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b234-110">Properties</span></span>

| <span data-ttu-id="1b234-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b234-111">Property</span></span>             | <span data-ttu-id="1b234-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b234-112">Type</span></span>                          | <span data-ttu-id="1b234-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b234-113">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1b234-114">createdBy</span><span class="sxs-lookup"><span data-stu-id="1b234-114">createdBy</span></span>            | <span data-ttu-id="1b234-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1b234-115">[identitySet][]</span></span>               | <span data-ttu-id="1b234-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="1b234-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b234-118">createdDateTime</span></span>      | <span data-ttu-id="1b234-119">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b234-119">dateTimeOffset</span></span>                | <span data-ttu-id="1b234-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="1b234-122">description</span><span class="sxs-lookup"><span data-stu-id="1b234-122">description</span></span>          | <span data-ttu-id="1b234-123">String</span><span class="sxs-lookup"><span data-stu-id="1b234-123">String</span></span>                        | <span data-ttu-id="1b234-124">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="1b234-124">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="1b234-125">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="1b234-125">Read-write.</span></span>
| <span data-ttu-id="1b234-126">driveType</span><span class="sxs-lookup"><span data-stu-id="1b234-126">driveType</span></span>            | <span data-ttu-id="1b234-127">String</span><span class="sxs-lookup"><span data-stu-id="1b234-127">String</span></span>                        | <span data-ttu-id="1b234-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="1b234-133">id</span><span class="sxs-lookup"><span data-stu-id="1b234-133">id</span></span>                   | <span data-ttu-id="1b234-134">String</span><span class="sxs-lookup"><span data-stu-id="1b234-134">String</span></span>                        | <span data-ttu-id="1b234-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="1b234-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1b234-137">lastModifiedBy</span></span>       | <span data-ttu-id="1b234-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1b234-138">[identitySet][]</span></span>               | <span data-ttu-id="1b234-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="1b234-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b234-141">lastModifiedDateTime</span></span> | <span data-ttu-id="1b234-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b234-142">dateTimeOffset</span></span>                | <span data-ttu-id="1b234-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="1b234-145">nome</span><span class="sxs-lookup"><span data-stu-id="1b234-145">name</span></span>                 | <span data-ttu-id="1b234-146">string</span><span class="sxs-lookup"><span data-stu-id="1b234-146">string</span></span>                        | <span data-ttu-id="1b234-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="1b234-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="1b234-149">owner</span><span class="sxs-lookup"><span data-stu-id="1b234-149">owner</span></span>                | [<span data-ttu-id="1b234-150">identitySet</span><span class="sxs-lookup"><span data-stu-id="1b234-150">identitySet</span></span>](identityset.md) | <span data-ttu-id="1b234-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="1b234-154">quota</span><span class="sxs-lookup"><span data-stu-id="1b234-154">quota</span></span>                | [<span data-ttu-id="1b234-155">quota</span><span class="sxs-lookup"><span data-stu-id="1b234-155">quota</span></span>](quota.md)             | <span data-ttu-id="1b234-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="1b234-159">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="1b234-159">sharepointIds</span></span>        | <span data-ttu-id="1b234-160">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="1b234-160">[sharepointIds][]</span></span>             | <span data-ttu-id="1b234-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="1b234-163">sistema</span><span class="sxs-lookup"><span data-stu-id="1b234-163">system</span></span>               | <span data-ttu-id="1b234-164">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="1b234-164">[systemFacet][]</span></span>               | <span data-ttu-id="1b234-165">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="1b234-165">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="1b234-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-166">Read-only.</span></span>
| <span data-ttu-id="1b234-167">webUrl</span><span class="sxs-lookup"><span data-stu-id="1b234-167">webUrl</span></span>               | <span data-ttu-id="1b234-168">string (url)</span><span class="sxs-lookup"><span data-stu-id="1b234-168">string (url)</span></span>                  | <span data-ttu-id="1b234-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="1b234-174">Relações</span><span class="sxs-lookup"><span data-stu-id="1b234-174">Relationships</span></span>

| <span data-ttu-id="1b234-175">Relação</span><span class="sxs-lookup"><span data-stu-id="1b234-175">Relationship</span></span> | <span data-ttu-id="1b234-176">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b234-176">Type</span></span>                                 | <span data-ttu-id="1b234-177">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b234-177">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="1b234-178">items</span><span class="sxs-lookup"><span data-stu-id="1b234-178">items</span></span>        | <span data-ttu-id="1b234-179">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b234-179">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="1b234-p115">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="1b234-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="1b234-183">root</span><span class="sxs-lookup"><span data-stu-id="1b234-183">root</span></span>         | [<span data-ttu-id="1b234-184">DriveItem</span><span class="sxs-lookup"><span data-stu-id="1b234-184">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="1b234-p116">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="1b234-187">special</span><span class="sxs-lookup"><span data-stu-id="1b234-187">special</span></span>      | <span data-ttu-id="1b234-188">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="1b234-188">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="1b234-189">Coleção de pastas comuns disponíveis no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="1b234-189">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="1b234-190">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-190">Read-only.</span></span> <span data-ttu-id="1b234-191">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1b234-191">Nullable.</span></span>
| <span data-ttu-id="1b234-192">list</span><span class="sxs-lookup"><span data-stu-id="1b234-192">list</span></span>         | [<span data-ttu-id="1b234-193">List</span><span class="sxs-lookup"><span data-stu-id="1b234-193">List</span></span>](list.md)                      | <span data-ttu-id="1b234-194">Para unidades no SharePoint, a lista de biblioteca de documentos subjacentes.</span><span class="sxs-lookup"><span data-stu-id="1b234-194">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="1b234-195">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b234-195">Read-only.</span></span> <span data-ttu-id="1b234-196">Anulável.</span><span class="sxs-lookup"><span data-stu-id="1b234-196">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="1b234-197">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b234-197">Methods</span></span>

|                        <span data-ttu-id="1b234-198">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="1b234-198">Common task</span></span>                         |         <span data-ttu-id="1b234-199">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="1b234-199">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="1b234-200">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="1b234-200">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="1b234-201">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="1b234-201">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="1b234-202">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="1b234-202">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="1b234-203">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="1b234-203">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="1b234-204">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="1b234-204">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="1b234-205">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="1b234-205">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="1b234-206">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="1b234-206">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive-get.md
[item-get]: ../api/driveitem-get.md
[item-changes]: ../api/driveitem-delta.md
[item-search]: ../api/driveitem-search.md
[item-children]: ../api/driveitem-list-children.md


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
