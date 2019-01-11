---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: b0ee801945a4b1d202b55d997d8cfc87a8dadff5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829152"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="1ae3e-102">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1ae3e-102">IdentitySet resource type</span></span>

<span data-ttu-id="1ae3e-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ae3e-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ae3e-105">JSON representation</span></span>

<span data-ttu-id="1ae3e-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="1ae3e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ae3e-107">Properties</span></span>

| <span data-ttu-id="1ae3e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ae3e-108">Property</span></span>    | <span data-ttu-id="1ae3e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ae3e-109">Type</span></span>                    | <span data-ttu-id="1ae3e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ae3e-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="1ae3e-111">application</span><span class="sxs-lookup"><span data-stu-id="1ae3e-111">application</span></span> | [<span data-ttu-id="1ae3e-112">Identity</span><span class="sxs-lookup"><span data-stu-id="1ae3e-112">Identity</span></span>](identity.md) | <span data-ttu-id="1ae3e-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="1ae3e-115">dispositivo</span><span class="sxs-lookup"><span data-stu-id="1ae3e-115">device</span></span>      | [<span data-ttu-id="1ae3e-116">Identity</span><span class="sxs-lookup"><span data-stu-id="1ae3e-116">Identity</span></span>](identity.md) | <span data-ttu-id="1ae3e-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="1ae3e-119">Usuário</span><span class="sxs-lookup"><span data-stu-id="1ae3e-119">user</span></span>        | [<span data-ttu-id="1ae3e-120">Identity</span><span class="sxs-lookup"><span data-stu-id="1ae3e-120">Identity</span></span>](identity.md) | <span data-ttu-id="1ae3e-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="1ae3e-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="1ae3e-123">Remarks</span></span> 

<span data-ttu-id="1ae3e-124">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="1ae3e-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
