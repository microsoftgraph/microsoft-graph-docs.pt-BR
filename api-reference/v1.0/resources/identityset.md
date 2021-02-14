---
author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
description: O recurso IdentitySet é uma coleção de chaves dos recursos identity.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e6f7aef915596e39173f286a3433e0114656e707
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239958"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="60355-103">Tipo de recurso IdentitySet</span><span class="sxs-lookup"><span data-stu-id="60355-103">IdentitySet resource type</span></span>

<span data-ttu-id="60355-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60355-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="60355-p101">O recurso **IdentitySet** é uma coleção de chaves dos recursos [identity](identity.md). É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="60355-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60355-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60355-107">JSON representation</span></span>

<span data-ttu-id="60355-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60355-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="60355-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60355-109">Properties</span></span>

| <span data-ttu-id="60355-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60355-110">Property</span></span>    | <span data-ttu-id="60355-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="60355-111">Type</span></span>                    | <span data-ttu-id="60355-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="60355-112">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="60355-113">application</span><span class="sxs-lookup"><span data-stu-id="60355-113">application</span></span> | [<span data-ttu-id="60355-114">Identity</span><span class="sxs-lookup"><span data-stu-id="60355-114">Identity</span></span>](identity.md) | <span data-ttu-id="60355-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="60355-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="60355-117">device</span><span class="sxs-lookup"><span data-stu-id="60355-117">device</span></span>      | [<span data-ttu-id="60355-118">Identity</span><span class="sxs-lookup"><span data-stu-id="60355-118">Identity</span></span>](identity.md) | <span data-ttu-id="60355-p103">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="60355-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="60355-121">user</span><span class="sxs-lookup"><span data-stu-id="60355-121">user</span></span>        | [<span data-ttu-id="60355-122">Identity</span><span class="sxs-lookup"><span data-stu-id="60355-122">Identity</span></span>](identity.md) | <span data-ttu-id="60355-p104">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="60355-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="60355-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="60355-125">Remarks</span></span> 

<span data-ttu-id="60355-126">Consulte [DriveItem](driveitem.md) para saber mais sobre o uso de recursos **IdentitySet**.</span><span class="sxs-lookup"><span data-stu-id="60355-126">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

