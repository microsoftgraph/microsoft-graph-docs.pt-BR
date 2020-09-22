---
author: JeremyKelley
description: O recurso baseItem é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos.
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6fbaf549cb9555c787cdd9077421ca1e3641aa04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089726"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="2961a-103">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="2961a-103">BaseItem resource type</span></span>

<span data-ttu-id="2961a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2961a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2961a-p101">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="2961a-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="2961a-107">drive</span><span class="sxs-lookup"><span data-stu-id="2961a-107">drive</span></span>](drive.md)
* [<span data-ttu-id="2961a-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="2961a-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="2961a-109">site</span><span class="sxs-lookup"><span data-stu-id="2961a-109">site</span></span>](site.md)
* [<span data-ttu-id="2961a-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="2961a-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="2961a-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2961a-111">JSON representation</span></span>

<span data-ttu-id="2961a-112">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="2961a-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2961a-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2961a-113">Properties</span></span>

| <span data-ttu-id="2961a-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2961a-114">Property</span></span>             | <span data-ttu-id="2961a-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2961a-115">Type</span></span>              | <span data-ttu-id="2961a-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2961a-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="2961a-117">id</span><span class="sxs-lookup"><span data-stu-id="2961a-117">id</span></span>                   | <span data-ttu-id="2961a-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2961a-118">string</span></span>            | <span data-ttu-id="2961a-p102">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="2961a-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="2961a-121">createdBy</span></span>            | <span data-ttu-id="2961a-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2961a-122">[identitySet][]</span></span>   | <span data-ttu-id="2961a-p103">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="2961a-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2961a-125">createdDateTime</span></span>      | <span data-ttu-id="2961a-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2961a-126">dateTimeOffset</span></span>    | <span data-ttu-id="2961a-p104">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="2961a-129">eTag</span><span class="sxs-lookup"><span data-stu-id="2961a-129">eTag</span></span>                 | <span data-ttu-id="2961a-130">string</span><span class="sxs-lookup"><span data-stu-id="2961a-130">string</span></span>            | <span data-ttu-id="2961a-p105">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="2961a-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2961a-133">lastModifiedBy</span></span>       | <span data-ttu-id="2961a-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="2961a-134">[identitySet][]</span></span>   | <span data-ttu-id="2961a-p106">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="2961a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2961a-137">lastModifiedDateTime</span></span> | <span data-ttu-id="2961a-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2961a-138">dateTimeOffset</span></span>    | <span data-ttu-id="2961a-p107">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="2961a-141">nome</span><span class="sxs-lookup"><span data-stu-id="2961a-141">name</span></span>                 | <span data-ttu-id="2961a-142">string</span><span class="sxs-lookup"><span data-stu-id="2961a-142">string</span></span>            | <span data-ttu-id="2961a-p108">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2961a-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="2961a-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="2961a-145">parentReference</span></span>      | <span data-ttu-id="2961a-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="2961a-146">[itemReference][]</span></span> | <span data-ttu-id="2961a-p109">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="2961a-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="2961a-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="2961a-149">webUrl</span></span>               | <span data-ttu-id="2961a-150">string (url)</span><span class="sxs-lookup"><span data-stu-id="2961a-150">string (url)</span></span>      | <span data-ttu-id="2961a-p110">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2961a-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="2961a-155">Comentários</span><span class="sxs-lookup"><span data-stu-id="2961a-155">Remarks</span></span>

<span data-ttu-id="2961a-156">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="2961a-156">The `baseItem` type is not expected to be used directly.</span></span>

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


