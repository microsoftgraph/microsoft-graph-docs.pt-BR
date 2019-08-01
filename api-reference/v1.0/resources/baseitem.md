---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2bde386a736805d52758f6d80e629c585f82d87e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029978"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="5f99c-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="5f99c-103">BaseItem resource type</span></span>

<span data-ttu-id="5f99c-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="5f99c-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="5f99c-106">drive</span><span class="sxs-lookup"><span data-stu-id="5f99c-106">drive</span></span>](drive.md)
* [<span data-ttu-id="5f99c-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="5f99c-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="5f99c-108">site</span><span class="sxs-lookup"><span data-stu-id="5f99c-108">site</span></span>](site.md)
* [<span data-ttu-id="5f99c-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="5f99c-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="5f99c-110">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f99c-110">JSON representation</span></span>

<span data-ttu-id="5f99c-111">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="5f99c-111">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5f99c-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f99c-112">Properties</span></span>

| <span data-ttu-id="5f99c-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f99c-113">Property</span></span>             | <span data-ttu-id="5f99c-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f99c-114">Type</span></span>              | <span data-ttu-id="5f99c-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f99c-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="5f99c-116">id</span><span class="sxs-lookup"><span data-stu-id="5f99c-116">id</span></span>                   | <span data-ttu-id="5f99c-117">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f99c-117">string</span></span>            | <span data-ttu-id="5f99c-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="5f99c-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="5f99c-120">createdBy</span></span>            | <span data-ttu-id="5f99c-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f99c-121">[identitySet][]</span></span>   | <span data-ttu-id="5f99c-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="5f99c-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f99c-124">createdDateTime</span></span>      | <span data-ttu-id="5f99c-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f99c-125">dateTimeOffset</span></span>    | <span data-ttu-id="5f99c-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="5f99c-128">description</span><span class="sxs-lookup"><span data-stu-id="5f99c-128">description</span></span>          | <span data-ttu-id="5f99c-129">String</span><span class="sxs-lookup"><span data-stu-id="5f99c-129">String</span></span>            | <span data-ttu-id="5f99c-130">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5f99c-130">Provides a user-visible description of the item.</span></span> <span data-ttu-id="5f99c-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5f99c-131">Optional.</span></span>                             |
| <span data-ttu-id="5f99c-132">eTag</span><span class="sxs-lookup"><span data-stu-id="5f99c-132">eTag</span></span>                 | <span data-ttu-id="5f99c-133">string</span><span class="sxs-lookup"><span data-stu-id="5f99c-133">string</span></span>            | <span data-ttu-id="5f99c-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="5f99c-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="5f99c-136">lastModifiedBy</span></span>       | <span data-ttu-id="5f99c-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="5f99c-137">[identitySet][]</span></span>   | <span data-ttu-id="5f99c-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="5f99c-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f99c-140">lastModifiedDateTime</span></span> | <span data-ttu-id="5f99c-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f99c-141">dateTimeOffset</span></span>    | <span data-ttu-id="5f99c-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="5f99c-144">nome</span><span class="sxs-lookup"><span data-stu-id="5f99c-144">name</span></span>                 | <span data-ttu-id="5f99c-145">string</span><span class="sxs-lookup"><span data-stu-id="5f99c-145">string</span></span>            | <span data-ttu-id="5f99c-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="5f99c-148">parentReference</span><span class="sxs-lookup"><span data-stu-id="5f99c-148">parentReference</span></span>      | <span data-ttu-id="5f99c-149">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="5f99c-149">[itemReference][]</span></span> | <span data-ttu-id="5f99c-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="5f99c-152">webUrl</span><span class="sxs-lookup"><span data-stu-id="5f99c-152">webUrl</span></span>               | <span data-ttu-id="5f99c-153">string (url)</span><span class="sxs-lookup"><span data-stu-id="5f99c-153">string (url)</span></span>      | <span data-ttu-id="5f99c-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="5f99c-156">Relações</span><span class="sxs-lookup"><span data-stu-id="5f99c-156">Relationships</span></span>

| <span data-ttu-id="5f99c-157">Relação</span><span class="sxs-lookup"><span data-stu-id="5f99c-157">Relationship</span></span>       | <span data-ttu-id="5f99c-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f99c-158">Type</span></span>     | <span data-ttu-id="5f99c-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f99c-159">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="5f99c-160">createdByUser</span><span class="sxs-lookup"><span data-stu-id="5f99c-160">createdByUser</span></span>      | <span data-ttu-id="5f99c-161">[user][]</span><span class="sxs-lookup"><span data-stu-id="5f99c-161">[user][]</span></span> | <span data-ttu-id="5f99c-162">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="5f99c-162">Identity of the user who created the item.</span></span> <span data-ttu-id="5f99c-163">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-163">Read-only.</span></span>
| <span data-ttu-id="5f99c-164">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="5f99c-164">lastModifiedByUser</span></span> | <span data-ttu-id="5f99c-165">[user][]</span><span class="sxs-lookup"><span data-stu-id="5f99c-165">[user][]</span></span> | <span data-ttu-id="5f99c-166">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5f99c-166">Identity of the user who last modified the item.</span></span> <span data-ttu-id="5f99c-167">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5f99c-167">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[Usuário]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="5f99c-171">Comentários</span><span class="sxs-lookup"><span data-stu-id="5f99c-171">Remarks</span></span>

<span data-ttu-id="5f99c-172">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="5f99c-172">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
