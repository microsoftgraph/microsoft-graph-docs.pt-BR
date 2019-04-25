---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567568"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="ca69d-102">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ca69d-102">IdentitySet resource type</span></span>

<span data-ttu-id="ca69d-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="ca69d-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca69d-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca69d-105">JSON representation</span></span>

<span data-ttu-id="ca69d-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca69d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ca69d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca69d-107">Properties</span></span>

| <span data-ttu-id="ca69d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca69d-108">Property</span></span>    | <span data-ttu-id="ca69d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca69d-109">Type</span></span>                    | <span data-ttu-id="ca69d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca69d-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="ca69d-111">application</span><span class="sxs-lookup"><span data-stu-id="ca69d-111">application</span></span> | [<span data-ttu-id="ca69d-112">Identidade</span><span class="sxs-lookup"><span data-stu-id="ca69d-112">Identity</span></span>](identity.md) | <span data-ttu-id="ca69d-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ca69d-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="ca69d-115">device</span><span class="sxs-lookup"><span data-stu-id="ca69d-115">device</span></span>      | [<span data-ttu-id="ca69d-116">Identidade</span><span class="sxs-lookup"><span data-stu-id="ca69d-116">Identity</span></span>](identity.md) | <span data-ttu-id="ca69d-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ca69d-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="ca69d-119">user</span><span class="sxs-lookup"><span data-stu-id="ca69d-119">user</span></span>        | [<span data-ttu-id="ca69d-120">Identity</span><span class="sxs-lookup"><span data-stu-id="ca69d-120">Identity</span></span>](identity.md) | <span data-ttu-id="ca69d-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="ca69d-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="ca69d-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca69d-123">Remarks</span></span> 

<span data-ttu-id="ca69d-124">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="ca69d-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
