---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c247891afed001977174f3de232a8b2385e0841
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075081"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="b0248-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="b0248-103">BaseItem resource type</span></span>

<span data-ttu-id="b0248-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0248-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0248-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="b0248-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="b0248-107">drive</span><span class="sxs-lookup"><span data-stu-id="b0248-107">drive</span></span>](drive.md)
* [<span data-ttu-id="b0248-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="b0248-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="b0248-109">site</span><span class="sxs-lookup"><span data-stu-id="b0248-109">site</span></span>](site.md)
* [<span data-ttu-id="b0248-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="b0248-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="b0248-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0248-111">JSON representation</span></span>

<span data-ttu-id="b0248-112">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="b0248-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b0248-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0248-113">Properties</span></span>

| <span data-ttu-id="b0248-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0248-114">Property</span></span>             | <span data-ttu-id="b0248-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0248-115">Type</span></span>              | <span data-ttu-id="b0248-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0248-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="b0248-117">id</span><span class="sxs-lookup"><span data-stu-id="b0248-117">id</span></span>                   | <span data-ttu-id="b0248-118">string</span><span class="sxs-lookup"><span data-stu-id="b0248-118">string</span></span>            | <span data-ttu-id="b0248-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="b0248-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="b0248-121">createdBy</span></span>            | <span data-ttu-id="b0248-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b0248-122">[identitySet][]</span></span>   | <span data-ttu-id="b0248-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="b0248-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0248-125">createdDateTime</span></span>      | <span data-ttu-id="b0248-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0248-126">dateTimeOffset</span></span>    | <span data-ttu-id="b0248-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="b0248-129">description</span><span class="sxs-lookup"><span data-stu-id="b0248-129">description</span></span>          | <span data-ttu-id="b0248-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0248-130">String</span></span>            | <span data-ttu-id="b0248-131">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b0248-131">Provides a user-visible description of the item.</span></span> <span data-ttu-id="b0248-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b0248-132">Optional.</span></span>                             |
| <span data-ttu-id="b0248-133">eTag</span><span class="sxs-lookup"><span data-stu-id="b0248-133">eTag</span></span>                 | <span data-ttu-id="b0248-134">string</span><span class="sxs-lookup"><span data-stu-id="b0248-134">string</span></span>            | <span data-ttu-id="b0248-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="b0248-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b0248-137">lastModifiedBy</span></span>       | <span data-ttu-id="b0248-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b0248-138">[identitySet][]</span></span>   | <span data-ttu-id="b0248-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="b0248-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0248-141">lastModifiedDateTime</span></span> | <span data-ttu-id="b0248-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0248-142">dateTimeOffset</span></span>    | <span data-ttu-id="b0248-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="b0248-145">nome</span><span class="sxs-lookup"><span data-stu-id="b0248-145">name</span></span>                 | <span data-ttu-id="b0248-146">string</span><span class="sxs-lookup"><span data-stu-id="b0248-146">string</span></span>            | <span data-ttu-id="b0248-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="b0248-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="b0248-149">parentReference</span><span class="sxs-lookup"><span data-stu-id="b0248-149">parentReference</span></span>      | <span data-ttu-id="b0248-150">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b0248-150">[itemReference][]</span></span> | <span data-ttu-id="b0248-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="b0248-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="b0248-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="b0248-153">webUrl</span></span>               | <span data-ttu-id="b0248-154">string (url)</span><span class="sxs-lookup"><span data-stu-id="b0248-154">string (url)</span></span>      | <span data-ttu-id="b0248-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="b0248-157">Relações</span><span class="sxs-lookup"><span data-stu-id="b0248-157">Relationships</span></span>

| <span data-ttu-id="b0248-158">Relação</span><span class="sxs-lookup"><span data-stu-id="b0248-158">Relationship</span></span>       | <span data-ttu-id="b0248-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0248-159">Type</span></span>     | <span data-ttu-id="b0248-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0248-160">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="b0248-161">createdByUser</span><span class="sxs-lookup"><span data-stu-id="b0248-161">createdByUser</span></span>      | <span data-ttu-id="b0248-162">[user][]</span><span class="sxs-lookup"><span data-stu-id="b0248-162">[user][]</span></span> | <span data-ttu-id="b0248-163">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="b0248-163">Identity of the user who created the item.</span></span> <span data-ttu-id="b0248-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-164">Read-only.</span></span>
| <span data-ttu-id="b0248-165">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="b0248-165">lastModifiedByUser</span></span> | <span data-ttu-id="b0248-166">[user][]</span><span class="sxs-lookup"><span data-stu-id="b0248-166">[user][]</span></span> | <span data-ttu-id="b0248-167">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0248-167">Identity of the user who last modified the item.</span></span> <span data-ttu-id="b0248-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b0248-168">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[Usuário]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="b0248-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0248-172">Remarks</span></span>

<span data-ttu-id="b0248-173">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="b0248-173">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

