---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 4d2bb5d92ebe06e79a68d69b949baec19a33a4c6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="identityset-resource-type"></a><span data-ttu-id="37bce-102">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="37bce-102">IdentitySet resource type</span></span>

<span data-ttu-id="37bce-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="37bce-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="37bce-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37bce-105">JSON representation</span></span>

<span data-ttu-id="37bce-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37bce-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="37bce-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37bce-107">Properties</span></span>

| <span data-ttu-id="37bce-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37bce-108">Property</span></span>    | <span data-ttu-id="37bce-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="37bce-109">Type</span></span>                    | <span data-ttu-id="37bce-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="37bce-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="37bce-111">application</span><span class="sxs-lookup"><span data-stu-id="37bce-111">application</span></span> | [<span data-ttu-id="37bce-112">Identity</span><span class="sxs-lookup"><span data-stu-id="37bce-112">Identity</span></span>](identity.md) | <span data-ttu-id="37bce-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="37bce-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="37bce-115">dispositivo</span><span class="sxs-lookup"><span data-stu-id="37bce-115">device</span></span>      | [<span data-ttu-id="37bce-116">Identity</span><span class="sxs-lookup"><span data-stu-id="37bce-116">Identity</span></span>](identity.md) | <span data-ttu-id="37bce-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="37bce-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="37bce-119">Usuário</span><span class="sxs-lookup"><span data-stu-id="37bce-119">user</span></span>        | [<span data-ttu-id="37bce-120">Identity</span><span class="sxs-lookup"><span data-stu-id="37bce-120">Identity</span></span>](identity.md) | <span data-ttu-id="37bce-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="37bce-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="37bce-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="37bce-123">Remarks</span></span> 

<span data-ttu-id="37bce-124">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="37bce-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
