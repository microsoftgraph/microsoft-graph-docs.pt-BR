---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 8e01d219fcc67c583fddba8d9893ed94a23c409b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481969"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="428ef-102">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="428ef-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="428ef-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="428ef-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="428ef-105">drive</span><span class="sxs-lookup"><span data-stu-id="428ef-105">drive</span></span>](drive.md)
* [<span data-ttu-id="428ef-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="428ef-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="428ef-107">site</span><span class="sxs-lookup"><span data-stu-id="428ef-107">site</span></span>](site.md)
* [<span data-ttu-id="428ef-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="428ef-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="428ef-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="428ef-109">JSON representation</span></span>

<span data-ttu-id="428ef-110">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="428ef-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="428ef-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="428ef-111">Properties</span></span>

| <span data-ttu-id="428ef-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="428ef-112">Property</span></span>             | <span data-ttu-id="428ef-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="428ef-113">Type</span></span>              | <span data-ttu-id="428ef-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="428ef-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="428ef-115">id</span><span class="sxs-lookup"><span data-stu-id="428ef-115">id</span></span>                   | <span data-ttu-id="428ef-116">string</span><span class="sxs-lookup"><span data-stu-id="428ef-116">string</span></span>            | <span data-ttu-id="428ef-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="428ef-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="428ef-119">createdBy</span></span>            | <span data-ttu-id="428ef-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="428ef-120">[identitySet][]</span></span>   | <span data-ttu-id="428ef-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="428ef-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="428ef-123">createdDateTime</span></span>      | <span data-ttu-id="428ef-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="428ef-124">dateTimeOffset</span></span>    | <span data-ttu-id="428ef-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="428ef-127">eTag</span><span class="sxs-lookup"><span data-stu-id="428ef-127">eTag</span></span>                 | <span data-ttu-id="428ef-128">string</span><span class="sxs-lookup"><span data-stu-id="428ef-128">string</span></span>            | <span data-ttu-id="428ef-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="428ef-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="428ef-131">lastModifiedBy</span></span>       | <span data-ttu-id="428ef-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="428ef-132">[identitySet][]</span></span>   | <span data-ttu-id="428ef-p106">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="428ef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="428ef-135">lastModifiedDateTime</span></span> | <span data-ttu-id="428ef-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="428ef-136">dateTimeOffset</span></span>    | <span data-ttu-id="428ef-p107">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="428ef-139">nome</span><span class="sxs-lookup"><span data-stu-id="428ef-139">name</span></span>                 | <span data-ttu-id="428ef-140">string</span><span class="sxs-lookup"><span data-stu-id="428ef-140">string</span></span>            | <span data-ttu-id="428ef-p108">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="428ef-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="428ef-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="428ef-143">parentReference</span></span>      | <span data-ttu-id="428ef-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="428ef-144">[itemReference][]</span></span> | <span data-ttu-id="428ef-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="428ef-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="428ef-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="428ef-147">webUrl</span></span>               | <span data-ttu-id="428ef-148">string (url)</span><span class="sxs-lookup"><span data-stu-id="428ef-148">string (url)</span></span>      | <span data-ttu-id="428ef-p110">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="428ef-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="428ef-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="428ef-153">Remarks</span></span>

<span data-ttu-id="428ef-154">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="428ef-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
