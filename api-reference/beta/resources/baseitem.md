---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: d70a75be0be4d7ecbd010288cb313b8394736932
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041078"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="0ea84-102">Tipo de recurso BaseItem</span><span class="sxs-lookup"><span data-stu-id="0ea84-102">BaseItem resource type</span></span>

> <span data-ttu-id="0ea84-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ea84-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ea84-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ea84-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0ea84-p102">O recurso **baseItem** é um recurso abstrato que contém um conjunto comum de propriedades compartilhado entre vários outros tipos de recursos. Recursos que derivam de **baseItem** incluem:</span><span class="sxs-lookup"><span data-stu-id="0ea84-p102">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="0ea84-107">drive</span><span class="sxs-lookup"><span data-stu-id="0ea84-107">drive</span></span>](drive.md)
* [<span data-ttu-id="0ea84-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="0ea84-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="0ea84-109">site</span><span class="sxs-lookup"><span data-stu-id="0ea84-109">site</span></span>](site.md)
* [<span data-ttu-id="0ea84-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="0ea84-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="0ea84-111">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ea84-111">JSON representation</span></span>

<span data-ttu-id="0ea84-112">Veja a seguir uma representação JSON de um recurso **baseItem**.</span><span class="sxs-lookup"><span data-stu-id="0ea84-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="0ea84-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ea84-113">Properties</span></span>

| <span data-ttu-id="0ea84-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ea84-114">Property</span></span>             | <span data-ttu-id="0ea84-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ea84-115">Type</span></span>              | <span data-ttu-id="0ea84-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ea84-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="0ea84-117">id</span><span class="sxs-lookup"><span data-stu-id="0ea84-117">id</span></span>                   | <span data-ttu-id="0ea84-118">string</span><span class="sxs-lookup"><span data-stu-id="0ea84-118">string</span></span>            | <span data-ttu-id="0ea84-p103">O identificador exclusivo da unidade. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p103">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="0ea84-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="0ea84-121">createdBy</span></span>            | <span data-ttu-id="0ea84-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0ea84-122">[identitySet][]</span></span>   | <span data-ttu-id="0ea84-p104">Identidade do usuário, dispositivo ou aplicativo que criou o item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p104">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="0ea84-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea84-125">createdDateTime</span></span>      | <span data-ttu-id="0ea84-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea84-126">dateTimeOffset</span></span>    | <span data-ttu-id="0ea84-p105">Data e hora de criação do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p105">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="0ea84-129">eTag</span><span class="sxs-lookup"><span data-stu-id="0ea84-129">eTag</span></span>                 | <span data-ttu-id="0ea84-130">string</span><span class="sxs-lookup"><span data-stu-id="0ea84-130">string</span></span>            | <span data-ttu-id="0ea84-p106">ETag do item. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="0ea84-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0ea84-133">lastModifiedBy</span></span>       | <span data-ttu-id="0ea84-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="0ea84-134">[identitySet][]</span></span>   | <span data-ttu-id="0ea84-p107">Identidade do usuário, dispositivo e aplicativo que modificou o item pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="0ea84-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ea84-137">lastModifiedDateTime</span></span> | <span data-ttu-id="0ea84-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ea84-138">dateTimeOffset</span></span>    | <span data-ttu-id="0ea84-p108">Data e hora em que o item foi modificado pela última vez. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="0ea84-141">name</span><span class="sxs-lookup"><span data-stu-id="0ea84-141">name</span></span>                 | <span data-ttu-id="0ea84-142">string</span><span class="sxs-lookup"><span data-stu-id="0ea84-142">string</span></span>            | <span data-ttu-id="0ea84-p109">O nome do item. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="0ea84-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="0ea84-145">parentReference</span></span>      | <span data-ttu-id="0ea84-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="0ea84-146">[itemReference][]</span></span> | <span data-ttu-id="0ea84-p110">Informações do pai, se o item tiver um pai. Leitura e gravação.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="0ea84-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="0ea84-149">webUrl</span></span>               | <span data-ttu-id="0ea84-150">string (url)</span><span class="sxs-lookup"><span data-stu-id="0ea84-150">string (url)</span></span>      | <span data-ttu-id="0ea84-p111">URL que exibe o recurso no navegador. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0ea84-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="0ea84-155">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ea84-155">Remarks</span></span>

<span data-ttu-id="0ea84-156">O tipo `baseItem` não deve ser usado diretamente.</span><span class="sxs-lookup"><span data-stu-id="0ea84-156">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
