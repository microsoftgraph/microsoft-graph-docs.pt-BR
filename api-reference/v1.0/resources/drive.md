---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
description: O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.
doc_type: resourcePageType
ms.openlocfilehash: 3b3d7d2d82ab2a6539ace2fa143ceaad55722336
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531565"
---
# <a name="drive-resource-type"></a><span data-ttu-id="ea527-103">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="ea527-103">Drive resource type</span></span>

<span data-ttu-id="ea527-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea527-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea527-105">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ea527-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="ea527-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="ea527-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea527-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea527-108">JSON representation</span></span>

<span data-ttu-id="ea527-109">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="ea527-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="ea527-110">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="ea527-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ea527-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea527-111">Properties</span></span>

| <span data-ttu-id="ea527-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea527-112">Property</span></span>             | <span data-ttu-id="ea527-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea527-113">Type</span></span>                          | <span data-ttu-id="ea527-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea527-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ea527-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="ea527-115">createdBy</span></span>            | <span data-ttu-id="ea527-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ea527-116">[identitySet][]</span></span>               | <span data-ttu-id="ea527-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="ea527-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea527-119">createdDateTime</span></span>      | <span data-ttu-id="ea527-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea527-120">dateTimeOffset</span></span>                | <span data-ttu-id="ea527-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="ea527-123">description</span><span class="sxs-lookup"><span data-stu-id="ea527-123">description</span></span>          | <span data-ttu-id="ea527-124">String</span><span class="sxs-lookup"><span data-stu-id="ea527-124">String</span></span>                        | <span data-ttu-id="ea527-125">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="ea527-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="ea527-126">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ea527-126">Read-write.</span></span>
| <span data-ttu-id="ea527-127">driveType</span><span class="sxs-lookup"><span data-stu-id="ea527-127">driveType</span></span>            | <span data-ttu-id="ea527-128">String</span><span class="sxs-lookup"><span data-stu-id="ea527-128">String</span></span>                        | <span data-ttu-id="ea527-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="ea527-134">id</span><span class="sxs-lookup"><span data-stu-id="ea527-134">id</span></span>                   | <span data-ttu-id="ea527-135">String</span><span class="sxs-lookup"><span data-stu-id="ea527-135">String</span></span>                        | <span data-ttu-id="ea527-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="ea527-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ea527-138">lastModifiedBy</span></span>       | <span data-ttu-id="ea527-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ea527-139">[identitySet][]</span></span>               | <span data-ttu-id="ea527-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="ea527-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea527-142">lastModifiedDateTime</span></span> | <span data-ttu-id="ea527-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea527-143">dateTimeOffset</span></span>                | <span data-ttu-id="ea527-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="ea527-146">nome</span><span class="sxs-lookup"><span data-stu-id="ea527-146">name</span></span>                 | <span data-ttu-id="ea527-147">string</span><span class="sxs-lookup"><span data-stu-id="ea527-147">string</span></span>                        | <span data-ttu-id="ea527-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ea527-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="ea527-150">owner</span><span class="sxs-lookup"><span data-stu-id="ea527-150">owner</span></span>                | [<span data-ttu-id="ea527-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="ea527-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="ea527-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="ea527-155">quota</span><span class="sxs-lookup"><span data-stu-id="ea527-155">quota</span></span>                | [<span data-ttu-id="ea527-156">quota</span><span class="sxs-lookup"><span data-stu-id="ea527-156">quota</span></span>](quota.md)             | <span data-ttu-id="ea527-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="ea527-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ea527-160">sharepointIds</span></span>        | <span data-ttu-id="ea527-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ea527-161">[sharepointIds][]</span></span>             | <span data-ttu-id="ea527-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ea527-164">sistema</span><span class="sxs-lookup"><span data-stu-id="ea527-164">system</span></span>               | <span data-ttu-id="ea527-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ea527-165">[systemFacet][]</span></span>               | <span data-ttu-id="ea527-166">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ea527-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="ea527-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-167">Read-only.</span></span>
| <span data-ttu-id="ea527-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="ea527-168">webUrl</span></span>               | <span data-ttu-id="ea527-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="ea527-169">string (url)</span></span>                  | <span data-ttu-id="ea527-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="ea527-175">Relações</span><span class="sxs-lookup"><span data-stu-id="ea527-175">Relationships</span></span>

| <span data-ttu-id="ea527-176">Relação</span><span class="sxs-lookup"><span data-stu-id="ea527-176">Relationship</span></span> | <span data-ttu-id="ea527-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea527-177">Type</span></span>                                 | <span data-ttu-id="ea527-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea527-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="ea527-179">items</span><span class="sxs-lookup"><span data-stu-id="ea527-179">items</span></span>        | <span data-ttu-id="ea527-180">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea527-180">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ea527-p115">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ea527-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ea527-184">root</span><span class="sxs-lookup"><span data-stu-id="ea527-184">root</span></span>         | [<span data-ttu-id="ea527-185">DriveItem</span><span class="sxs-lookup"><span data-stu-id="ea527-185">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="ea527-p116">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="ea527-188">special</span><span class="sxs-lookup"><span data-stu-id="ea527-188">special</span></span>      | <span data-ttu-id="ea527-189">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ea527-189">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ea527-190">Coleção de pastas comuns disponíveis no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="ea527-190">Collection of common folders available in OneDrive.</span></span> <span data-ttu-id="ea527-191">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-191">Read-only.</span></span> <span data-ttu-id="ea527-192">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ea527-192">Nullable.</span></span>
| <span data-ttu-id="ea527-193">list</span><span class="sxs-lookup"><span data-stu-id="ea527-193">list</span></span>         | [<span data-ttu-id="ea527-194">List</span><span class="sxs-lookup"><span data-stu-id="ea527-194">List</span></span>](list.md)                      | <span data-ttu-id="ea527-195">Para unidades no SharePoint, a lista de biblioteca de documentos subjacentes.</span><span class="sxs-lookup"><span data-stu-id="ea527-195">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="ea527-196">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea527-196">Read-only.</span></span> <span data-ttu-id="ea527-197">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ea527-197">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="ea527-198">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea527-198">Methods</span></span>

|                        <span data-ttu-id="ea527-199">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="ea527-199">Common task</span></span>                         |         <span data-ttu-id="ea527-200">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="ea527-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="ea527-201">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="ea527-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="ea527-202">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="ea527-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="ea527-203">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="ea527-203">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="ea527-204">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="ea527-204">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="ea527-205">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="ea527-205">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="ea527-206">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="ea527-206">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="ea527-207">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="ea527-207">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
