---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 3b9744d8b652f0374c71f5304c326ba862c288a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929127"
---
# <a name="drive-resource-type"></a><span data-ttu-id="ef977-102">Tipo de unidade de recurso</span><span class="sxs-lookup"><span data-stu-id="ef977-102">Drive resource type</span></span>

<span data-ttu-id="ef977-103">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ef977-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="ef977-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="ef977-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef977-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ef977-106">JSON representation</span></span>

<span data-ttu-id="ef977-107">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="ef977-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="ef977-108">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="ef977-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ef977-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ef977-109">Properties</span></span>

| <span data-ttu-id="ef977-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef977-110">Property</span></span>             | <span data-ttu-id="ef977-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef977-111">Type</span></span>                          | <span data-ttu-id="ef977-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef977-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ef977-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="ef977-113">createdBy</span></span>            | <span data-ttu-id="ef977-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ef977-114">[identitySet][]</span></span>               | <span data-ttu-id="ef977-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="ef977-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef977-117">createdDateTime</span></span>      | <span data-ttu-id="ef977-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef977-118">dateTimeOffset</span></span>                | <span data-ttu-id="ef977-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="ef977-121">description</span><span class="sxs-lookup"><span data-stu-id="ef977-121">description</span></span>          | <span data-ttu-id="ef977-122">String</span><span class="sxs-lookup"><span data-stu-id="ef977-122">String</span></span>                        | <span data-ttu-id="ef977-123">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="ef977-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="ef977-124">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ef977-124">Read-write.</span></span>
| <span data-ttu-id="ef977-125">driveType</span><span class="sxs-lookup"><span data-stu-id="ef977-125">driveType</span></span>            | <span data-ttu-id="ef977-126">String</span><span class="sxs-lookup"><span data-stu-id="ef977-126">String</span></span>                        | <span data-ttu-id="ef977-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="ef977-132">id</span><span class="sxs-lookup"><span data-stu-id="ef977-132">id</span></span>                   | <span data-ttu-id="ef977-133">String</span><span class="sxs-lookup"><span data-stu-id="ef977-133">String</span></span>                        | <span data-ttu-id="ef977-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="ef977-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ef977-136">lastModifiedBy</span></span>       | <span data-ttu-id="ef977-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ef977-137">[identitySet][]</span></span>               | <span data-ttu-id="ef977-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="ef977-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef977-140">lastModifiedDateTime</span></span> | <span data-ttu-id="ef977-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef977-141">dateTimeOffset</span></span>                | <span data-ttu-id="ef977-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="ef977-144">nome</span><span class="sxs-lookup"><span data-stu-id="ef977-144">name</span></span>                 | <span data-ttu-id="ef977-145">string</span><span class="sxs-lookup"><span data-stu-id="ef977-145">string</span></span>                        | <span data-ttu-id="ef977-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="ef977-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="ef977-148">owner</span><span class="sxs-lookup"><span data-stu-id="ef977-148">owner</span></span>                | [<span data-ttu-id="ef977-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef977-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="ef977-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="ef977-153">quota</span><span class="sxs-lookup"><span data-stu-id="ef977-153">quota</span></span>                | [<span data-ttu-id="ef977-154">quota</span><span class="sxs-lookup"><span data-stu-id="ef977-154">quota</span></span>](quota.md)             | <span data-ttu-id="ef977-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="ef977-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ef977-158">sharepointIds</span></span>        | <span data-ttu-id="ef977-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ef977-159">[sharepointIds][]</span></span>             | <span data-ttu-id="ef977-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ef977-162">system</span><span class="sxs-lookup"><span data-stu-id="ef977-162">system</span></span>               | <span data-ttu-id="ef977-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ef977-163">[systemFacet][]</span></span>               | <span data-ttu-id="ef977-164">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="ef977-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="ef977-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-165">Read-only.</span></span>
| <span data-ttu-id="ef977-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="ef977-166">webUrl</span></span>               | <span data-ttu-id="ef977-167">string (url)</span><span class="sxs-lookup"><span data-stu-id="ef977-167">string (url)</span></span>                  | <span data-ttu-id="ef977-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="ef977-173">Relações</span><span class="sxs-lookup"><span data-stu-id="ef977-173">Relationships</span></span>

| <span data-ttu-id="ef977-174">Relação</span><span class="sxs-lookup"><span data-stu-id="ef977-174">Relationship</span></span> | <span data-ttu-id="ef977-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef977-175">Type</span></span>                                 | <span data-ttu-id="ef977-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef977-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="ef977-177">items</span><span class="sxs-lookup"><span data-stu-id="ef977-177">items</span></span>        | <span data-ttu-id="ef977-178">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ef977-178">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ef977-p115">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef977-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ef977-182">root</span><span class="sxs-lookup"><span data-stu-id="ef977-182">root</span></span>         | [<span data-ttu-id="ef977-183">DriveItem</span><span class="sxs-lookup"><span data-stu-id="ef977-183">DriveItem</span></span>](driveitem.md)            | <span data-ttu-id="ef977-p116">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="ef977-186">special</span><span class="sxs-lookup"><span data-stu-id="ef977-186">special</span></span>      | <span data-ttu-id="ef977-187">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="ef977-187">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="ef977-p117">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef977-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="ef977-191">lista</span><span class="sxs-lookup"><span data-stu-id="ef977-191">list</span></span>         | [<span data-ttu-id="ef977-192">List</span><span class="sxs-lookup"><span data-stu-id="ef977-192">List</span></span>](list.md)                      | <span data-ttu-id="ef977-193">Para as unidades no SharePoint, a lista da biblioteca de documentos subjacentes.</span><span class="sxs-lookup"><span data-stu-id="ef977-193">For drives in SharePoint, the underlying document library list.</span></span> <span data-ttu-id="ef977-194">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef977-194">Read-only.</span></span> <span data-ttu-id="ef977-195">Anulável.</span><span class="sxs-lookup"><span data-stu-id="ef977-195">Nullable.</span></span>

## <a name="methods"></a><span data-ttu-id="ef977-196">Métodos</span><span class="sxs-lookup"><span data-stu-id="ef977-196">Methods</span></span>

|                        <span data-ttu-id="ef977-197">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="ef977-197">Common task</span></span>                         |         <span data-ttu-id="ef977-198">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="ef977-198">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="ef977-199">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="ef977-199">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="ef977-200">[Recuperar pasta raiz padrão da Unidade do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="ef977-200">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="ef977-201">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="ef977-201">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="ef977-202">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="ef977-202">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="ef977-203">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="ef977-203">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="ef977-204">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="ef977-204">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="ef977-205">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="ef977-205">In the previous table, the examples use `/drive`, but other pathes are valid too.</span></span>

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
