---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: 10b39bd5747e10ea4340bb5b4c54df0f94eb4229
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547141"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="1abd4-102">tipo de recurso identityset</span><span class="sxs-lookup"><span data-stu-id="1abd4-102">identitySet resource type</span></span>

<span data-ttu-id="1abd4-103">O \*\*\*\* recurso identityset é uma coleção com chave de recursos de [identidade](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="1abd4-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>
<span data-ttu-id="1abd4-104">É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="1abd4-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1abd4-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1abd4-105">JSON representation</span></span>

<span data-ttu-id="1abd4-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1abd4-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
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
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="1abd4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1abd4-107">Properties</span></span>

| <span data-ttu-id="1abd4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1abd4-108">Property</span></span>    | <span data-ttu-id="1abd4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1abd4-109">Type</span></span>                    | <span data-ttu-id="1abd4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1abd4-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="1abd4-111">application</span><span class="sxs-lookup"><span data-stu-id="1abd4-111">application</span></span> | [<span data-ttu-id="1abd4-112">Identidade</span><span class="sxs-lookup"><span data-stu-id="1abd4-112">Identity</span></span>](identity.md) | <span data-ttu-id="1abd4-p102">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1abd4-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="1abd4-115">conversa</span><span class="sxs-lookup"><span data-stu-id="1abd4-115">conversation</span></span>| [<span data-ttu-id="1abd4-116">Identity</span><span class="sxs-lookup"><span data-stu-id="1abd4-116">Identity</span></span>](identity.md) | <span data-ttu-id="1abd4-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1abd4-117">Optional.</span></span> <span data-ttu-id="1abd4-118">A equipe ou canal associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="1abd4-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="1abd4-119">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="1abd4-119">conversationIdentityType</span></span>| [<span data-ttu-id="1abd4-120">Identity</span><span class="sxs-lookup"><span data-stu-id="1abd4-120">Identity</span></span>](identity.md) | <span data-ttu-id="1abd4-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1abd4-121">Optional.</span></span> <span data-ttu-id="1abd4-122">Indica se a propriedade de **conversa** identifica uma equipe ou um canal.</span><span class="sxs-lookup"><span data-stu-id="1abd4-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="1abd4-123">device</span><span class="sxs-lookup"><span data-stu-id="1abd4-123">device</span></span>      | [<span data-ttu-id="1abd4-124">Identidade</span><span class="sxs-lookup"><span data-stu-id="1abd4-124">Identity</span></span>](identity.md) | <span data-ttu-id="1abd4-p105">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1abd4-p105">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="1abd4-127">phone</span><span class="sxs-lookup"><span data-stu-id="1abd4-127">phone</span></span>       | [<span data-ttu-id="1abd4-128">identity</span><span class="sxs-lookup"><span data-stu-id="1abd4-128">identity</span></span>](identity.md) | <span data-ttu-id="1abd4-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1abd4-129">Optional.</span></span> <span data-ttu-id="1abd4-130">O número de telefone associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="1abd4-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="1abd4-131">user</span><span class="sxs-lookup"><span data-stu-id="1abd4-131">user</span></span>        | [<span data-ttu-id="1abd4-132">Identity</span><span class="sxs-lookup"><span data-stu-id="1abd4-132">Identity</span></span>](identity.md) | <span data-ttu-id="1abd4-p107">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="1abd4-p107">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="1abd4-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="1abd4-135">Remarks</span></span> 

<span data-ttu-id="1abd4-136">ConFira [chamada](call.md) para uso \*\*\*\* de recursos identityset.</span><span class="sxs-lookup"><span data-stu-id="1abd4-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
