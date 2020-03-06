---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 181895c835544540387c96856c9cbbfb3b5e4f5d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532005"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="77025-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="77025-103">BaseItem resource type</span></span>

<span data-ttu-id="77025-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77025-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77025-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="77025-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="77025-107">drive</span><span class="sxs-lookup"><span data-stu-id="77025-107">drive</span></span>](drive.md)
* [<span data-ttu-id="77025-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="77025-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="77025-109">site</span><span class="sxs-lookup"><span data-stu-id="77025-109">site</span></span>](site.md)
* [<span data-ttu-id="77025-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="77025-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="77025-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77025-111">JSON representation</span></span>

<span data-ttu-id="77025-112">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="77025-112">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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

## <a name="properties"></a><span data-ttu-id="77025-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77025-113">Properties</span></span>

| <span data-ttu-id="77025-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77025-114">Property</span></span>             | <span data-ttu-id="77025-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="77025-115">Type</span></span>              | <span data-ttu-id="77025-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="77025-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="77025-117">id</span><span class="sxs-lookup"><span data-stu-id="77025-117">id</span></span>                   | <span data-ttu-id="77025-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77025-118">string</span></span>            | <span data-ttu-id="77025-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="77025-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="77025-121">createdBy</span></span>            | <span data-ttu-id="77025-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="77025-122">[identitySet][]</span></span>   | <span data-ttu-id="77025-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="77025-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77025-125">createdDateTime</span></span>      | <span data-ttu-id="77025-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77025-126">dateTimeOffset</span></span>    | <span data-ttu-id="77025-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="77025-129">description</span><span class="sxs-lookup"><span data-stu-id="77025-129">description</span></span>          | <span data-ttu-id="77025-130">String</span><span class="sxs-lookup"><span data-stu-id="77025-130">String</span></span>            | <span data-ttu-id="77025-131">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="77025-131">Provides a user-visible description of the item.</span></span> <span data-ttu-id="77025-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="77025-132">Optional.</span></span>                             |
| <span data-ttu-id="77025-133">eTag</span><span class="sxs-lookup"><span data-stu-id="77025-133">eTag</span></span>                 | <span data-ttu-id="77025-134">string</span><span class="sxs-lookup"><span data-stu-id="77025-134">string</span></span>            | <span data-ttu-id="77025-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="77025-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="77025-137">lastModifiedBy</span></span>       | <span data-ttu-id="77025-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="77025-138">[identitySet][]</span></span>   | <span data-ttu-id="77025-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="77025-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77025-141">lastModifiedDateTime</span></span> | <span data-ttu-id="77025-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77025-142">dateTimeOffset</span></span>    | <span data-ttu-id="77025-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="77025-145">nome</span><span class="sxs-lookup"><span data-stu-id="77025-145">name</span></span>                 | <span data-ttu-id="77025-146">string</span><span class="sxs-lookup"><span data-stu-id="77025-146">string</span></span>            | <span data-ttu-id="77025-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="77025-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="77025-149">parentReference</span><span class="sxs-lookup"><span data-stu-id="77025-149">parentReference</span></span>      | <span data-ttu-id="77025-150">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="77025-150">[itemReference][]</span></span> | <span data-ttu-id="77025-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="77025-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="77025-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="77025-153">webUrl</span></span>               | <span data-ttu-id="77025-154">string (url)</span><span class="sxs-lookup"><span data-stu-id="77025-154">string (url)</span></span>      | <span data-ttu-id="77025-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="77025-157">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="77025-157">Relationships</span></span>

| <span data-ttu-id="77025-158">Relação</span><span class="sxs-lookup"><span data-stu-id="77025-158">Relationship</span></span>       | <span data-ttu-id="77025-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="77025-159">Type</span></span>     | <span data-ttu-id="77025-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="77025-160">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="77025-161">createdByUser</span><span class="sxs-lookup"><span data-stu-id="77025-161">createdByUser</span></span>      | <span data-ttu-id="77025-162">[user][]</span><span class="sxs-lookup"><span data-stu-id="77025-162">[user][]</span></span> | <span data-ttu-id="77025-163">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="77025-163">Identity of the user who created the item.</span></span> <span data-ttu-id="77025-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-164">Read-only.</span></span>
| <span data-ttu-id="77025-165">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="77025-165">lastModifiedByUser</span></span> | <span data-ttu-id="77025-166">[user][]</span><span class="sxs-lookup"><span data-stu-id="77025-166">[user][]</span></span> | <span data-ttu-id="77025-167">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="77025-167">Identity of the user who last modified the item.</span></span> <span data-ttu-id="77025-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="77025-168">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="77025-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="77025-172">Remarks</span></span>

<span data-ttu-id="77025-173">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="77025-173">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
