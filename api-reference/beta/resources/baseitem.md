---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 5bc3aab8460c1d0c6774d2f8afda13c4fc89f69d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521583"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="5b0cb-102">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="5b0cb-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b0cb-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="5b0cb-105">drive</span><span class="sxs-lookup"><span data-stu-id="5b0cb-105">drive</span></span>](drive.md)
* [<span data-ttu-id="5b0cb-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="5b0cb-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="5b0cb-107">site</span><span class="sxs-lookup"><span data-stu-id="5b0cb-107">site</span></span>](site.md)
* [<span data-ttu-id="5b0cb-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="5b0cb-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="5b0cb-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b0cb-109">JSON representation</span></span>

<span data-ttu-id="5b0cb-110">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-110">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5b0cb-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b0cb-111">Properties</span></span>

| <span data-ttu-id="5b0cb-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b0cb-112">Property</span></span>             | <span data-ttu-id="5b0cb-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b0cb-113">Type</span></span>              | <span data-ttu-id="5b0cb-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b0cb-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b0cb-115">id</span><span class="sxs-lookup"><span data-stu-id="5b0cb-115">id</span></span>                   | <span data-ttu-id="5b0cb-116">string</span><span class="sxs-lookup"><span data-stu-id="5b0cb-116">string</span></span>            | <span data-ttu-id="5b0cb-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="5b0cb-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="5b0cb-119">createdBy</span></span>            | <span data-ttu-id="5b0cb-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5b0cb-120">[identitySet][]</span></span>   | <span data-ttu-id="5b0cb-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="5b0cb-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b0cb-123">createdDateTime</span></span>      | <span data-ttu-id="5b0cb-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b0cb-124">dateTimeOffset</span></span>    | <span data-ttu-id="5b0cb-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="5b0cb-127">eTag</span><span class="sxs-lookup"><span data-stu-id="5b0cb-127">eTag</span></span>                 | <span data-ttu-id="5b0cb-128">string</span><span class="sxs-lookup"><span data-stu-id="5b0cb-128">string</span></span>            | <span data-ttu-id="5b0cb-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="5b0cb-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5b0cb-131">lastModifiedBy</span></span>       | <span data-ttu-id="5b0cb-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5b0cb-132">[identitySet][]</span></span>   | <span data-ttu-id="5b0cb-p106">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="5b0cb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b0cb-135">lastModifiedDateTime</span></span> | <span data-ttu-id="5b0cb-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b0cb-136">dateTimeOffset</span></span>    | <span data-ttu-id="5b0cb-p107">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="5b0cb-139">nome</span><span class="sxs-lookup"><span data-stu-id="5b0cb-139">name</span></span>                 | <span data-ttu-id="5b0cb-140">string</span><span class="sxs-lookup"><span data-stu-id="5b0cb-140">string</span></span>            | <span data-ttu-id="5b0cb-p108">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="5b0cb-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="5b0cb-143">parentReference</span></span>      | <span data-ttu-id="5b0cb-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5b0cb-144">[itemReference][]</span></span> | <span data-ttu-id="5b0cb-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="5b0cb-147">webUrl</span><span class="sxs-lookup"><span data-stu-id="5b0cb-147">webUrl</span></span>               | <span data-ttu-id="5b0cb-148">string (url)</span><span class="sxs-lookup"><span data-stu-id="5b0cb-148">string (url)</span></span>      | <span data-ttu-id="5b0cb-p110">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="5b0cb-153">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b0cb-153">Remarks</span></span>

<span data-ttu-id="5b0cb-154">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="5b0cb-154">The `baseItem` type is not expected to be used directly.</span></span>

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
