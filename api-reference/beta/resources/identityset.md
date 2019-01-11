---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 63178fc9add3d097b7e8aaf0c5c2a697a91eaeed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807018"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="ec8a0-102">tipo de recurso de identitySet</span><span class="sxs-lookup"><span data-stu-id="ec8a0-102">identitySet resource type</span></span>

<span data-ttu-id="ec8a0-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec8a0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec8a0-105">JSON representation</span></span>

<span data-ttu-id="ec8a0-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="ec8a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec8a0-107">Properties</span></span>

| <span data-ttu-id="ec8a0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec8a0-108">Property</span></span>    | <span data-ttu-id="ec8a0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec8a0-109">Type</span></span>                    | <span data-ttu-id="ec8a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec8a0-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="ec8a0-111">application</span><span class="sxs-lookup"><span data-stu-id="ec8a0-111">application</span></span> | [<span data-ttu-id="ec8a0-112">Identity</span><span class="sxs-lookup"><span data-stu-id="ec8a0-112">Identity</span></span>](identity.md) | <span data-ttu-id="ec8a0-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="ec8a0-115">dispositivo</span><span class="sxs-lookup"><span data-stu-id="ec8a0-115">device</span></span>      | [<span data-ttu-id="ec8a0-116">Identity</span><span class="sxs-lookup"><span data-stu-id="ec8a0-116">Identity</span></span>](identity.md) | <span data-ttu-id="ec8a0-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="ec8a0-119">phone</span><span class="sxs-lookup"><span data-stu-id="ec8a0-119">phone</span></span>       | [<span data-ttu-id="ec8a0-120">identity</span><span class="sxs-lookup"><span data-stu-id="ec8a0-120">identity</span></span>](identity.md) | <span data-ttu-id="ec8a0-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-121">Optional.</span></span> <span data-ttu-id="ec8a0-122">O número de telefone associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="ec8a0-123">user</span><span class="sxs-lookup"><span data-stu-id="ec8a0-123">user</span></span>        | [<span data-ttu-id="ec8a0-124">Identity</span><span class="sxs-lookup"><span data-stu-id="ec8a0-124">Identity</span></span>](identity.md) | <span data-ttu-id="ec8a0-p105">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ec8a0-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="ec8a0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec8a0-127">Remarks</span></span> 

<span data-ttu-id="ec8a0-128">Consulte a [chamada](call.md) para o uso de recursos de **IdentitySet** .</span><span class="sxs-lookup"><span data-stu-id="ec8a0-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
