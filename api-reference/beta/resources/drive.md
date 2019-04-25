---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 82a14f6462604b732119b90d037b2fab711df5af
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507837"
---
# <a name="drive-resource-type"></a><span data-ttu-id="2f698-102">tipo de recurso de unidade</span><span class="sxs-lookup"><span data-stu-id="2f698-102">drive resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f698-103">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2f698-103">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="2f698-p101">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="2f698-p101">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f698-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f698-106">JSON representation</span></span>

<span data-ttu-id="2f698-107">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="2f698-107">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="2f698-108">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="2f698-108">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "following": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="2f698-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f698-109">Properties</span></span>

| <span data-ttu-id="2f698-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f698-110">Property</span></span>             | <span data-ttu-id="2f698-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f698-111">Type</span></span>                          | <span data-ttu-id="2f698-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f698-112">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2f698-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="2f698-113">createdBy</span></span>            | <span data-ttu-id="2f698-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2f698-114">[identitySet][]</span></span>               | <span data-ttu-id="2f698-p102">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p102">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="2f698-117">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f698-117">createdDateTime</span></span>      | <span data-ttu-id="2f698-118">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f698-118">dateTimeOffset</span></span>                | <span data-ttu-id="2f698-p103">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p103">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="2f698-121">description</span><span class="sxs-lookup"><span data-stu-id="2f698-121">description</span></span>          | <span data-ttu-id="2f698-122">String</span><span class="sxs-lookup"><span data-stu-id="2f698-122">String</span></span>                        | <span data-ttu-id="2f698-123">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="2f698-123">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="2f698-124">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2f698-124">Read-write.</span></span>
| <span data-ttu-id="2f698-125">driveType</span><span class="sxs-lookup"><span data-stu-id="2f698-125">driveType</span></span>            | <span data-ttu-id="2f698-126">String</span><span class="sxs-lookup"><span data-stu-id="2f698-126">String</span></span>                        | <span data-ttu-id="2f698-p105">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p105">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="2f698-132">id</span><span class="sxs-lookup"><span data-stu-id="2f698-132">id</span></span>                   | <span data-ttu-id="2f698-133">String</span><span class="sxs-lookup"><span data-stu-id="2f698-133">String</span></span>                        | <span data-ttu-id="2f698-p106">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p106">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="2f698-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2f698-136">lastModifiedBy</span></span>       | <span data-ttu-id="2f698-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2f698-137">[identitySet][]</span></span>               | <span data-ttu-id="2f698-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="2f698-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f698-140">lastModifiedDateTime</span></span> | <span data-ttu-id="2f698-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f698-141">dateTimeOffset</span></span>                | <span data-ttu-id="2f698-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p108">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="2f698-144">nome</span><span class="sxs-lookup"><span data-stu-id="2f698-144">name</span></span>                 | <span data-ttu-id="2f698-145">string</span><span class="sxs-lookup"><span data-stu-id="2f698-145">string</span></span>                        | <span data-ttu-id="2f698-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2f698-p109">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="2f698-148">owner</span><span class="sxs-lookup"><span data-stu-id="2f698-148">owner</span></span>                | [<span data-ttu-id="2f698-149">identitySet</span><span class="sxs-lookup"><span data-stu-id="2f698-149">identitySet</span></span>](identityset.md) | <span data-ttu-id="2f698-p110">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p110">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="2f698-153">quota</span><span class="sxs-lookup"><span data-stu-id="2f698-153">quota</span></span>                | [<span data-ttu-id="2f698-154">quota</span><span class="sxs-lookup"><span data-stu-id="2f698-154">quota</span></span>](quota.md)             | <span data-ttu-id="2f698-p111">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p111">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="2f698-158">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="2f698-158">sharepointIds</span></span>        | <span data-ttu-id="2f698-159">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="2f698-159">[sharepointIds][]</span></span>             | <span data-ttu-id="2f698-p112">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p112">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="2f698-162">sistema</span><span class="sxs-lookup"><span data-stu-id="2f698-162">system</span></span>               | <span data-ttu-id="2f698-163">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="2f698-163">[systemFacet][]</span></span>               | <span data-ttu-id="2f698-164">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="2f698-164">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="2f698-165">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-165">Read-only.</span></span>
| <span data-ttu-id="2f698-166">webUrl</span><span class="sxs-lookup"><span data-stu-id="2f698-166">webUrl</span></span>               | <span data-ttu-id="2f698-167">string (url)</span><span class="sxs-lookup"><span data-stu-id="2f698-167">string (url)</span></span>                  | <span data-ttu-id="2f698-p114">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p114">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="2f698-173">Relações</span><span class="sxs-lookup"><span data-stu-id="2f698-173">Relationships</span></span>

| <span data-ttu-id="2f698-174">Relação</span><span class="sxs-lookup"><span data-stu-id="2f698-174">Relationship</span></span> | <span data-ttu-id="2f698-175">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f698-175">Type</span></span>                                 | <span data-ttu-id="2f698-176">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f698-176">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="2f698-177">activities</span><span class="sxs-lookup"><span data-stu-id="2f698-177">activities</span></span>   | <span data-ttu-id="2f698-178">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="2f698-178">[itemActivity][] collection</span></span>          | <span data-ttu-id="2f698-179">A lista de atividades recentes que ocorreram nesta unidade.</span><span class="sxs-lookup"><span data-stu-id="2f698-179">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="2f698-180">items</span><span class="sxs-lookup"><span data-stu-id="2f698-180">items</span></span>        | <span data-ttu-id="2f698-181">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f698-181">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="2f698-p115">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f698-p115">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="2f698-185">root</span><span class="sxs-lookup"><span data-stu-id="2f698-185">root</span></span>         | [<span data-ttu-id="2f698-186">driveitem</span><span class="sxs-lookup"><span data-stu-id="2f698-186">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="2f698-p116">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f698-p116">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="2f698-189">special</span><span class="sxs-lookup"><span data-stu-id="2f698-189">special</span></span>      | <span data-ttu-id="2f698-190">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f698-190">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="2f698-p117">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2f698-p117">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="2f698-194">seguindo</span><span class="sxs-lookup"><span data-stu-id="2f698-194">following</span></span>    | <span data-ttu-id="2f698-195">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2f698-195">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="2f698-196">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="2f698-196">The list of items the user is following.</span></span> <span data-ttu-id="2f698-197">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="2f698-197">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="2f698-198">Métodos</span><span class="sxs-lookup"><span data-stu-id="2f698-198">Methods</span></span>

|                        <span data-ttu-id="2f698-199">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="2f698-199">Common task</span></span>                         |         <span data-ttu-id="2f698-200">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="2f698-200">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="2f698-201">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="2f698-201">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="2f698-202">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="2f698-202">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="2f698-203">[Listar atividades sob a Unidade][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="2f698-203">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="2f698-204">[Listar itens seguidos][drive-following]</span><span class="sxs-lookup"><span data-stu-id="2f698-204">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="2f698-205">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="2f698-205">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="2f698-206">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="2f698-206">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="2f698-207">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="2f698-207">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="2f698-208">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="2f698-208">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="2f698-209">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos também são válidos.</span><span class="sxs-lookup"><span data-stu-id="2f698-209">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/drive.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
