---
author: JeremyKelley
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 38e697e4a991871bd592cc891dcd131e845572fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013140"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="54e20-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="54e20-103">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54e20-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="54e20-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="54e20-106">drive</span><span class="sxs-lookup"><span data-stu-id="54e20-106">drive</span></span>](drive.md)
* [<span data-ttu-id="54e20-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="54e20-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="54e20-108">site</span><span class="sxs-lookup"><span data-stu-id="54e20-108">site</span></span>](site.md)
* [<span data-ttu-id="54e20-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="54e20-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="54e20-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54e20-110">JSON representation</span></span>

<span data-ttu-id="54e20-111">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="54e20-111">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "abstract": true
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

## <a name="properties"></a><span data-ttu-id="54e20-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54e20-112">Properties</span></span>

| <span data-ttu-id="54e20-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54e20-113">Property</span></span>             | <span data-ttu-id="54e20-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="54e20-114">Type</span></span>              | <span data-ttu-id="54e20-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="54e20-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="54e20-116">id</span><span class="sxs-lookup"><span data-stu-id="54e20-116">id</span></span>                   | <span data-ttu-id="54e20-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="54e20-117">string</span></span>            | <span data-ttu-id="54e20-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="54e20-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="54e20-120">createdBy</span></span>            | <span data-ttu-id="54e20-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="54e20-121">[identitySet][]</span></span>   | <span data-ttu-id="54e20-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="54e20-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="54e20-124">createdDateTime</span></span>      | <span data-ttu-id="54e20-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e20-125">dateTimeOffset</span></span>    | <span data-ttu-id="54e20-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="54e20-128">eTag</span><span class="sxs-lookup"><span data-stu-id="54e20-128">eTag</span></span>                 | <span data-ttu-id="54e20-129">string</span><span class="sxs-lookup"><span data-stu-id="54e20-129">string</span></span>            | <span data-ttu-id="54e20-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="54e20-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="54e20-132">lastModifiedBy</span></span>       | <span data-ttu-id="54e20-133">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="54e20-133">[identitySet][]</span></span>   | <span data-ttu-id="54e20-p106">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="54e20-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54e20-136">lastModifiedDateTime</span></span> | <span data-ttu-id="54e20-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="54e20-137">dateTimeOffset</span></span>    | <span data-ttu-id="54e20-p107">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="54e20-140">nome</span><span class="sxs-lookup"><span data-stu-id="54e20-140">name</span></span>                 | <span data-ttu-id="54e20-141">string</span><span class="sxs-lookup"><span data-stu-id="54e20-141">string</span></span>            | <span data-ttu-id="54e20-p108">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="54e20-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="54e20-144">parentReference</span><span class="sxs-lookup"><span data-stu-id="54e20-144">parentReference</span></span>      | <span data-ttu-id="54e20-145">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="54e20-145">[itemReference][]</span></span> | <span data-ttu-id="54e20-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="54e20-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="54e20-148">webUrl</span><span class="sxs-lookup"><span data-stu-id="54e20-148">webUrl</span></span>               | <span data-ttu-id="54e20-149">string (url)</span><span class="sxs-lookup"><span data-stu-id="54e20-149">string (url)</span></span>      | <span data-ttu-id="54e20-p110">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="54e20-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="54e20-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="54e20-154">Remarks</span></span>

<span data-ttu-id="54e20-155">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="54e20-155">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": []
}
-->
