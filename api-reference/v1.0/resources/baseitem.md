---
author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 717426f29b8c466af5799871fcc12cf4cd8bdf65
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239090"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="d9b8e-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="d9b8e-103">BaseItem resource type</span></span>

<span data-ttu-id="d9b8e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9b8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9b8e-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="d9b8e-107">drive</span><span class="sxs-lookup"><span data-stu-id="d9b8e-107">drive</span></span>](drive.md)
* [<span data-ttu-id="d9b8e-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="d9b8e-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="d9b8e-109">site</span><span class="sxs-lookup"><span data-stu-id="d9b8e-109">site</span></span>](site.md)
* [<span data-ttu-id="d9b8e-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="d9b8e-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="d9b8e-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9b8e-111">JSON representation</span></span>

<span data-ttu-id="d9b8e-112">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d9b8e-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9b8e-113">Properties</span></span>

| <span data-ttu-id="d9b8e-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9b8e-114">Property</span></span>             | <span data-ttu-id="d9b8e-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b8e-115">Type</span></span>              | <span data-ttu-id="d9b8e-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b8e-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="d9b8e-117">id</span><span class="sxs-lookup"><span data-stu-id="d9b8e-117">id</span></span>                   | <span data-ttu-id="d9b8e-118">string</span><span class="sxs-lookup"><span data-stu-id="d9b8e-118">string</span></span>            | <span data-ttu-id="d9b8e-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="d9b8e-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="d9b8e-121">createdBy</span></span>            | <span data-ttu-id="d9b8e-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d9b8e-122">[identitySet][]</span></span>   | <span data-ttu-id="d9b8e-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="d9b8e-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9b8e-125">createdDateTime</span></span>      | <span data-ttu-id="d9b8e-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9b8e-126">dateTimeOffset</span></span>    | <span data-ttu-id="d9b8e-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="d9b8e-129">description</span><span class="sxs-lookup"><span data-stu-id="d9b8e-129">description</span></span>          | <span data-ttu-id="d9b8e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9b8e-130">String</span></span>            | <span data-ttu-id="d9b8e-131">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-131">Provides a user-visible description of the item.</span></span> <span data-ttu-id="d9b8e-132">Opcional.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-132">Optional.</span></span>                             |
| <span data-ttu-id="d9b8e-133">eTag</span><span class="sxs-lookup"><span data-stu-id="d9b8e-133">eTag</span></span>                 | <span data-ttu-id="d9b8e-134">string</span><span class="sxs-lookup"><span data-stu-id="d9b8e-134">string</span></span>            | <span data-ttu-id="d9b8e-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="d9b8e-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d9b8e-137">lastModifiedBy</span></span>       | <span data-ttu-id="d9b8e-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d9b8e-138">[identitySet][]</span></span>   | <span data-ttu-id="d9b8e-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="d9b8e-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9b8e-141">lastModifiedDateTime</span></span> | <span data-ttu-id="d9b8e-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9b8e-142">dateTimeOffset</span></span>    | <span data-ttu-id="d9b8e-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="d9b8e-145">nome</span><span class="sxs-lookup"><span data-stu-id="d9b8e-145">name</span></span>                 | <span data-ttu-id="d9b8e-146">string</span><span class="sxs-lookup"><span data-stu-id="d9b8e-146">string</span></span>            | <span data-ttu-id="d9b8e-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="d9b8e-149">parentReference</span><span class="sxs-lookup"><span data-stu-id="d9b8e-149">parentReference</span></span>      | <span data-ttu-id="d9b8e-150">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="d9b8e-150">[itemReference][]</span></span> | <span data-ttu-id="d9b8e-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="d9b8e-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="d9b8e-153">webUrl</span></span>               | <span data-ttu-id="d9b8e-154">string (url)</span><span class="sxs-lookup"><span data-stu-id="d9b8e-154">string (url)</span></span>      | <span data-ttu-id="d9b8e-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="d9b8e-157">Relações</span><span class="sxs-lookup"><span data-stu-id="d9b8e-157">Relationships</span></span>

| <span data-ttu-id="d9b8e-158">Relação</span><span class="sxs-lookup"><span data-stu-id="d9b8e-158">Relationship</span></span>       | <span data-ttu-id="d9b8e-159">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9b8e-159">Type</span></span>     | <span data-ttu-id="d9b8e-160">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9b8e-160">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="d9b8e-161">createdByUser</span><span class="sxs-lookup"><span data-stu-id="d9b8e-161">createdByUser</span></span>      | <span data-ttu-id="d9b8e-162">[user][]</span><span class="sxs-lookup"><span data-stu-id="d9b8e-162">[user][]</span></span> | <span data-ttu-id="d9b8e-163">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-163">Identity of the user who created the item.</span></span> <span data-ttu-id="d9b8e-164">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-164">Read-only.</span></span>
| <span data-ttu-id="d9b8e-165">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="d9b8e-165">lastModifiedByUser</span></span> | <span data-ttu-id="d9b8e-166">[user][]</span><span class="sxs-lookup"><span data-stu-id="d9b8e-166">[user][]</span></span> | <span data-ttu-id="d9b8e-167">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-167">Identity of the user who last modified the item.</span></span> <span data-ttu-id="d9b8e-168">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-168">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="d9b8e-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9b8e-172">Remarks</span></span>

<span data-ttu-id="d9b8e-173">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="d9b8e-173">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

