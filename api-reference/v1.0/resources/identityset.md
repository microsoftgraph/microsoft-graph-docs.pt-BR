---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: O recurso IdentitySet é uma coleção de chaves dos recursos identity.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0a5d53769dc023e79ac9f50db2c085647775cab0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531338"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="fcc03-103">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fcc03-103">IdentitySet resource type</span></span>

<span data-ttu-id="fcc03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcc03-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcc03-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="fcc03-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fcc03-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fcc03-107">JSON representation</span></span>

<span data-ttu-id="fcc03-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fcc03-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fcc03-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fcc03-109">Properties</span></span>

| <span data-ttu-id="fcc03-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fcc03-110">Property</span></span>    | <span data-ttu-id="fcc03-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcc03-111">Type</span></span>                    | <span data-ttu-id="fcc03-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcc03-112">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="fcc03-113">application</span><span class="sxs-lookup"><span data-stu-id="fcc03-113">application</span></span> | [<span data-ttu-id="fcc03-114">Identidade</span><span class="sxs-lookup"><span data-stu-id="fcc03-114">Identity</span></span>](identity.md) | <span data-ttu-id="fcc03-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="fcc03-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="fcc03-117">device</span><span class="sxs-lookup"><span data-stu-id="fcc03-117">device</span></span>      | [<span data-ttu-id="fcc03-118">Identidade</span><span class="sxs-lookup"><span data-stu-id="fcc03-118">Identity</span></span>](identity.md) | <span data-ttu-id="fcc03-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="fcc03-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="fcc03-121">user</span><span class="sxs-lookup"><span data-stu-id="fcc03-121">user</span></span>        | [<span data-ttu-id="fcc03-122">Identity</span><span class="sxs-lookup"><span data-stu-id="fcc03-122">Identity</span></span>](identity.md) | <span data-ttu-id="fcc03-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="fcc03-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="fcc03-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="fcc03-125">Remarks</span></span> 

<span data-ttu-id="fcc03-126">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="fcc03-126">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
