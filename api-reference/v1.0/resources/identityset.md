---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: O recurso IdentitySet é uma coleção de chaves dos recursos identity.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f1176f133f51432899a1fb6ddab964f04e658c69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030216"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="b4621-103">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b4621-103">IdentitySet resource type</span></span>

<span data-ttu-id="b4621-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="b4621-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4621-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4621-106">JSON representation</span></span>

<span data-ttu-id="b4621-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4621-107">Here is a JSON representation of the resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="b4621-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4621-108">Properties</span></span>

| <span data-ttu-id="b4621-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4621-109">Property</span></span>    | <span data-ttu-id="b4621-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4621-110">Type</span></span>                    | <span data-ttu-id="b4621-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4621-111">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="b4621-112">application</span><span class="sxs-lookup"><span data-stu-id="b4621-112">application</span></span> | [<span data-ttu-id="b4621-113">Identidade</span><span class="sxs-lookup"><span data-stu-id="b4621-113">Identity</span></span>](identity.md) | <span data-ttu-id="b4621-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="b4621-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="b4621-116">device</span><span class="sxs-lookup"><span data-stu-id="b4621-116">device</span></span>      | [<span data-ttu-id="b4621-117">Identidade</span><span class="sxs-lookup"><span data-stu-id="b4621-117">Identity</span></span>](identity.md) | <span data-ttu-id="b4621-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="b4621-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="b4621-120">user</span><span class="sxs-lookup"><span data-stu-id="b4621-120">user</span></span>        | [<span data-ttu-id="b4621-121">Identity</span><span class="sxs-lookup"><span data-stu-id="b4621-121">Identity</span></span>](identity.md) | <span data-ttu-id="b4621-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="b4621-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="b4621-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b4621-124">Remarks</span></span> 

<span data-ttu-id="b4621-125">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="b4621-125">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
