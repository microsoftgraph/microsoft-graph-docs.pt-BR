---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Unidade
localization_priority: Priority
ms.openlocfilehash: 684a200d38aea52054bedb9eb4357c28e03b37e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840828"
---
# <a name="drive-resource-type"></a><span data-ttu-id="2adb4-102">tipo de recurso de unidade</span><span class="sxs-lookup"><span data-stu-id="2adb4-102">drive resource type</span></span>

> <span data-ttu-id="2adb4-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2adb4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2adb4-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2adb4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2adb4-105">O recurso drive é o objeto de nível superior que representa o OneDrive de um usuário ou uma biblioteca de documentos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2adb4-105">The drive resource is the top level object representing a user's OneDrive or a document library in SharePoint.</span></span>

<span data-ttu-id="2adb4-p102">Os usuários do OneDrive sempre terão pelo menos uma unidade disponível, sua unidade padrão. Usuários sem uma licença do OneDrive talvez não tenham uma unidade padrão disponível.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p102">OneDrive users will always have at least one drive available, their default drive. Users without a OneDrive license may not have a default drive available.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2adb4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2adb4-108">JSON representation</span></span>

<span data-ttu-id="2adb4-109">Veja a seguir uma representação JSON de um recurso Drive.</span><span class="sxs-lookup"><span data-stu-id="2adb4-109">Here is a JSON representation of a Drive resource.</span></span>

<span data-ttu-id="2adb4-110">O recurso **drive** é derivado de [**baseItem**](baseitem.md) e herda propriedades desse recurso.</span><span class="sxs-lookup"><span data-stu-id="2adb4-110">The **drive** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2adb4-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2adb4-111">Properties</span></span>

| <span data-ttu-id="2adb4-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2adb4-112">Property</span></span>             | <span data-ttu-id="2adb4-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adb4-113">Type</span></span>                          | <span data-ttu-id="2adb4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adb4-114">Description</span></span>                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2adb4-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="2adb4-115">createdBy</span></span>            | <span data-ttu-id="2adb4-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2adb4-116">[identitySet][]</span></span>               | <span data-ttu-id="2adb4-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>                                                                                                                                                  |
| <span data-ttu-id="2adb4-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2adb4-119">createdDateTime</span></span>      | <span data-ttu-id="2adb4-120">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2adb4-120">dateTimeOffset</span></span>                | <span data-ttu-id="2adb4-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p104">Date and time of item creation. Read-only.</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="2adb4-123">description</span><span class="sxs-lookup"><span data-stu-id="2adb4-123">description</span></span>          | <span data-ttu-id="2adb4-124">String</span><span class="sxs-lookup"><span data-stu-id="2adb4-124">String</span></span>                        | <span data-ttu-id="2adb4-125">Fornecer uma descrição visível para os usuários da unidade.</span><span class="sxs-lookup"><span data-stu-id="2adb4-125">Provide a user-visible description of the drive.</span></span> <span data-ttu-id="2adb4-126">Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2adb4-126">Read-write.</span></span>
| <span data-ttu-id="2adb4-127">driveType</span><span class="sxs-lookup"><span data-stu-id="2adb4-127">driveType</span></span>            | <span data-ttu-id="2adb4-128">String</span><span class="sxs-lookup"><span data-stu-id="2adb4-128">String</span></span>                        | <span data-ttu-id="2adb4-p106">Descreve o tipo de unidade representado por esse recurso. As unidades pessoais do OneDrive retornarão `personal`. O OneDrive for Business retornará `business`. As bibliotecas de documentos do SharePoint retornarão `documentLibrary`. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p106">Describes the type of drive represented by this resource. OneDrive personal drives will return `personal`. OneDrive for Business will return `business`. SharePoint document libraries will return `documentLibrary`. Read-only.</span></span> |
| <span data-ttu-id="2adb4-134">id</span><span class="sxs-lookup"><span data-stu-id="2adb4-134">id</span></span>                   | <span data-ttu-id="2adb4-135">String</span><span class="sxs-lookup"><span data-stu-id="2adb4-135">String</span></span>                        | <span data-ttu-id="2adb4-p107">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p107">The unique identifier of the drive. Read-only.</span></span>                                                                                                                                                                                   |
| <span data-ttu-id="2adb4-138">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2adb4-138">lastModifiedBy</span></span>       | <span data-ttu-id="2adb4-139">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2adb4-139">[identitySet][]</span></span>               | <span data-ttu-id="2adb4-p108">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p108">Identity of the user, device, and application which last modified the item. Read-only.</span></span>                                                                                                                                           |
| <span data-ttu-id="2adb4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2adb4-142">lastModifiedDateTime</span></span> | <span data-ttu-id="2adb4-143">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2adb4-143">dateTimeOffset</span></span>                | <span data-ttu-id="2adb4-p109">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p109">Date and time the item was last modified. Read-only.</span></span>                                                                                                                                                                             |
| <span data-ttu-id="2adb4-146">name</span><span class="sxs-lookup"><span data-stu-id="2adb4-146">name</span></span>                 | <span data-ttu-id="2adb4-147">string</span><span class="sxs-lookup"><span data-stu-id="2adb4-147">string</span></span>                        | <span data-ttu-id="2adb4-p110">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p110">The name of the item. Read-write.</span></span>                                                                                                                                                                                                |
| <span data-ttu-id="2adb4-150">owner</span><span class="sxs-lookup"><span data-stu-id="2adb4-150">owner</span></span>                | [<span data-ttu-id="2adb4-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="2adb4-151">identitySet</span></span>](identityset.md) | <span data-ttu-id="2adb4-p111">Opcional. A conta do usuário que é proprietário da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p111">Optional. The user account that owns the drive. Read-only.</span></span>                                                                                                                                                                       |
| <span data-ttu-id="2adb4-155">quota</span><span class="sxs-lookup"><span data-stu-id="2adb4-155">quota</span></span>                | [<span data-ttu-id="2adb4-156">quota</span><span class="sxs-lookup"><span data-stu-id="2adb4-156">quota</span></span>](quota.md)             | <span data-ttu-id="2adb4-p112">Opcional. Informações sobre a cota de espaço de armazenamento da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p112">Optional. Information about the drive's storage space quota. Read-only.</span></span>                                                                                                                                                          |
| <span data-ttu-id="2adb4-160">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="2adb4-160">sharepointIds</span></span>        | <span data-ttu-id="2adb4-161">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="2adb4-161">[sharepointIds][]</span></span>             | <span data-ttu-id="2adb4-p113">Retorna os identificadores úteis para fins de compatibilidade do REST do SharePoint. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p113">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                                                                                                                                                         |
| <span data-ttu-id="2adb4-164">system</span><span class="sxs-lookup"><span data-stu-id="2adb4-164">system</span></span>               | <span data-ttu-id="2adb4-165">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="2adb4-165">[systemFacet][]</span></span>               | <span data-ttu-id="2adb4-166">Se estiver presente, indica que se trata de uma unidade gerenciada pelo sistema.</span><span class="sxs-lookup"><span data-stu-id="2adb4-166">If present, indicates that this is a system-managed drive.</span></span> <span data-ttu-id="2adb4-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-167">Read-only.</span></span>
| <span data-ttu-id="2adb4-168">webUrl</span><span class="sxs-lookup"><span data-stu-id="2adb4-168">webUrl</span></span>               | <span data-ttu-id="2adb4-169">string (url)</span><span class="sxs-lookup"><span data-stu-id="2adb4-169">string (url)</span></span>                  | <span data-ttu-id="2adb4-p115">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p115">URL that displays the resource in the browser. Read-only.</span></span>                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a><span data-ttu-id="2adb4-175">Relações</span><span class="sxs-lookup"><span data-stu-id="2adb4-175">Relationships</span></span>

| <span data-ttu-id="2adb4-176">Relação</span><span class="sxs-lookup"><span data-stu-id="2adb4-176">Relationship</span></span> | <span data-ttu-id="2adb4-177">Tipo</span><span class="sxs-lookup"><span data-stu-id="2adb4-177">Type</span></span>                                 | <span data-ttu-id="2adb4-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="2adb4-178">Description</span></span>
|:-------------|:-------------------------------------|:-----------------------
| <span data-ttu-id="2adb4-179">activities</span><span class="sxs-lookup"><span data-stu-id="2adb4-179">activities</span></span>   | <span data-ttu-id="2adb4-180">Conjunto [itemActivity][]</span><span class="sxs-lookup"><span data-stu-id="2adb4-180">[itemActivity][] collection</span></span>          | <span data-ttu-id="2adb4-181">A lista de atividades recentes que ocorreram nesta unidade.</span><span class="sxs-lookup"><span data-stu-id="2adb4-181">The list of recent activities that took place under this drive.</span></span>
| <span data-ttu-id="2adb4-182">items</span><span class="sxs-lookup"><span data-stu-id="2adb4-182">items</span></span>        | <span data-ttu-id="2adb4-183">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2adb4-183">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="2adb4-p116">Todos os itens contidos na unidade. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p116">All items contained in the drive. Read-only. Nullable.</span></span>
| <span data-ttu-id="2adb4-187">root</span><span class="sxs-lookup"><span data-stu-id="2adb4-187">root</span></span>         | [<span data-ttu-id="2adb4-188">driveitem</span><span class="sxs-lookup"><span data-stu-id="2adb4-188">driveitem</span></span>](driveitem.md)            | <span data-ttu-id="2adb4-p117">A pasta raiz da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p117">The root folder of the drive. Read-only.</span></span>
| <span data-ttu-id="2adb4-191">special</span><span class="sxs-lookup"><span data-stu-id="2adb4-191">special</span></span>      | <span data-ttu-id="2adb4-192">Coleção [driveitem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2adb4-192">[driveitem](driveitem.md) collection</span></span> | <span data-ttu-id="2adb4-p118">Coleção de pastas comuns disponíveis no OneDrive. Somente leitura. Anulável.</span><span class="sxs-lookup"><span data-stu-id="2adb4-p118">Collection of common folders available in OneDrive. Read-only. Nullable.</span></span>
| <span data-ttu-id="2adb4-196">seguir</span><span class="sxs-lookup"><span data-stu-id="2adb4-196">following</span></span>    | <span data-ttu-id="2adb4-197">Coleção [DriveItem](driveitem.md)</span><span class="sxs-lookup"><span data-stu-id="2adb4-197">[DriveItem](driveitem.md) collection</span></span> | <span data-ttu-id="2adb4-198">A lista de itens que o usuário está seguindo.</span><span class="sxs-lookup"><span data-stu-id="2adb4-198">The list of items the user is following.</span></span> <span data-ttu-id="2adb4-199">Somente no OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="2adb4-199">Only in OneDrive for Business.</span></span>

## <a name="methods"></a><span data-ttu-id="2adb4-200">Métodos</span><span class="sxs-lookup"><span data-stu-id="2adb4-200">Methods</span></span>

|                        <span data-ttu-id="2adb4-201">Tarefa comum</span><span class="sxs-lookup"><span data-stu-id="2adb4-201">Common task</span></span>                         |         <span data-ttu-id="2adb4-202">Método HTTP</span><span class="sxs-lookup"><span data-stu-id="2adb4-202">HTTP method</span></span>         |
| :--------------------------------------------------------- | :-------------------------- |
| <span data-ttu-id="2adb4-203">[Recuperar metadados de outra Unidade][drive-get]</span><span class="sxs-lookup"><span data-stu-id="2adb4-203">[Get Drive metadata of another Drive][drive-get]</span></span>           | `GET /drives/{drive-id}`    |
| <span data-ttu-id="2adb4-204">[Recuperar a pasta raiz da Unidade padrão do usuário][item-get]</span><span class="sxs-lookup"><span data-stu-id="2adb4-204">[Get root folder for user's default Drive][item-get]</span></span>       | `GET /drive/root`           |
| <span data-ttu-id="2adb4-205">[Lista de atividades sob a Unidade][drive-activities]</span><span class="sxs-lookup"><span data-stu-id="2adb4-205">[List activities under the Drive][drive-activities]</span></span>        | `GET /drive/activities`     |
| <span data-ttu-id="2adb4-206">[Lista seguido de itens][drive-following]</span><span class="sxs-lookup"><span data-stu-id="2adb4-206">[List followed Items][drive-following]</span></span>                     | `GET /drive/following`      |
| <span data-ttu-id="2adb4-207">[Listar filhos na Unidade][item-children]</span><span class="sxs-lookup"><span data-stu-id="2adb4-207">[List children under the Drive][item-children]</span></span>             | `GET /drive/root/children`  |
| <span data-ttu-id="2adb4-208">[Listar alterações de todos os Itens na Unidade][item-changes]</span><span class="sxs-lookup"><span data-stu-id="2adb4-208">[List changes for all Items in the Drive][item-changes]</span></span>    | `GET /drive/root/delta`     |
| <span data-ttu-id="2adb4-209">[Pesquisar Itens na Unidade][item-search]</span><span class="sxs-lookup"><span data-stu-id="2adb4-209">[Search for Items in the Drive][item-search]</span></span>               | `GET /drive/root/search`    |
| [<span data-ttu-id="2adb4-210">Acessar pasta especial</span><span class="sxs-lookup"><span data-stu-id="2adb4-210">Access special folder</span></span>](../api/drive-get-specialfolder.md) | `GET /drive/special/{name}` |

<span data-ttu-id="2adb4-211">Na tabela anterior, os exemplos usam `/drive`, mas outros caminhos são muito válidos.</span><span class="sxs-lookup"><span data-stu-id="2adb4-211">In the previous table, the examples use `/drive`, but other paths are valid too.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
