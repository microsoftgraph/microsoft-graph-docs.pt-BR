---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: ae22b0a36acb46c2a9d872f224c0a6d4c567782c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569330"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="dd73c-102">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="dd73c-102">BaseItem resource type</span></span>

<span data-ttu-id="dd73c-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="dd73c-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="dd73c-105">drive</span><span class="sxs-lookup"><span data-stu-id="dd73c-105">drive</span></span>](drive.md)
* [<span data-ttu-id="dd73c-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="dd73c-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="dd73c-107">site</span><span class="sxs-lookup"><span data-stu-id="dd73c-107">site</span></span>](site.md)
* [<span data-ttu-id="dd73c-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="dd73c-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="dd73c-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd73c-109">JSON representation</span></span>

<span data-ttu-id="dd73c-110">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="dd73c-110">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd73c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd73c-111">Properties</span></span>

| <span data-ttu-id="dd73c-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd73c-112">Property</span></span>             | <span data-ttu-id="dd73c-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd73c-113">Type</span></span>              | <span data-ttu-id="dd73c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd73c-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="dd73c-115">id</span><span class="sxs-lookup"><span data-stu-id="dd73c-115">id</span></span>                   | <span data-ttu-id="dd73c-116">string</span><span class="sxs-lookup"><span data-stu-id="dd73c-116">string</span></span>            | <span data-ttu-id="dd73c-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="dd73c-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="dd73c-119">createdBy</span></span>            | <span data-ttu-id="dd73c-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dd73c-120">[identitySet][]</span></span>   | <span data-ttu-id="dd73c-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="dd73c-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd73c-123">createdDateTime</span></span>      | <span data-ttu-id="dd73c-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd73c-124">dateTimeOffset</span></span>    | <span data-ttu-id="dd73c-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="dd73c-127">description</span><span class="sxs-lookup"><span data-stu-id="dd73c-127">description</span></span>          | <span data-ttu-id="dd73c-128">String</span><span class="sxs-lookup"><span data-stu-id="dd73c-128">String</span></span>            | <span data-ttu-id="dd73c-129">Fornece uma descrição do item visível para o usuário.</span><span class="sxs-lookup"><span data-stu-id="dd73c-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="dd73c-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="dd73c-130">Optional.</span></span>                             |
| <span data-ttu-id="dd73c-131">eTag</span><span class="sxs-lookup"><span data-stu-id="dd73c-131">eTag</span></span>                 | <span data-ttu-id="dd73c-132">string</span><span class="sxs-lookup"><span data-stu-id="dd73c-132">string</span></span>            | <span data-ttu-id="dd73c-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="dd73c-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dd73c-135">lastModifiedBy</span></span>       | <span data-ttu-id="dd73c-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="dd73c-136">[identitySet][]</span></span>   | <span data-ttu-id="dd73c-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="dd73c-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd73c-139">lastModifiedDateTime</span></span> | <span data-ttu-id="dd73c-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd73c-140">dateTimeOffset</span></span>    | <span data-ttu-id="dd73c-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="dd73c-143">nome</span><span class="sxs-lookup"><span data-stu-id="dd73c-143">name</span></span>                 | <span data-ttu-id="dd73c-144">string</span><span class="sxs-lookup"><span data-stu-id="dd73c-144">string</span></span>            | <span data-ttu-id="dd73c-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="dd73c-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="dd73c-147">parentReference</span></span>      | <span data-ttu-id="dd73c-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="dd73c-148">[itemReference][]</span></span> | <span data-ttu-id="dd73c-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="dd73c-151">webUrl</span><span class="sxs-lookup"><span data-stu-id="dd73c-151">webUrl</span></span>               | <span data-ttu-id="dd73c-152">string (url)</span><span class="sxs-lookup"><span data-stu-id="dd73c-152">string (url)</span></span>      | <span data-ttu-id="dd73c-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="dd73c-155">Relações</span><span class="sxs-lookup"><span data-stu-id="dd73c-155">Relationships</span></span>

| <span data-ttu-id="dd73c-156">Relação</span><span class="sxs-lookup"><span data-stu-id="dd73c-156">Relationship</span></span>       | <span data-ttu-id="dd73c-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd73c-157">Type</span></span>     | <span data-ttu-id="dd73c-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd73c-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="dd73c-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="dd73c-159">createdByUser</span></span>      | <span data-ttu-id="dd73c-160">[user][]</span><span class="sxs-lookup"><span data-stu-id="dd73c-160">[user][]</span></span> | <span data-ttu-id="dd73c-161">A identidade do usuário que criou o item.</span><span class="sxs-lookup"><span data-stu-id="dd73c-161">Identity of the user who created the item.</span></span> <span data-ttu-id="dd73c-162">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-162">Read-only.</span></span>
| <span data-ttu-id="dd73c-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="dd73c-163">lastModifiedByUser</span></span> | <span data-ttu-id="dd73c-164">[user][]</span><span class="sxs-lookup"><span data-stu-id="dd73c-164">[user][]</span></span> | <span data-ttu-id="dd73c-165">A identidade do usuário que modificou o item pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dd73c-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="dd73c-166">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dd73c-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[Usuário]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="dd73c-170">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd73c-170">Remarks</span></span>

<span data-ttu-id="dd73c-171">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="dd73c-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
