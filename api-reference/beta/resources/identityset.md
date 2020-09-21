---
author: JeremyKelley
description: O recurso identityset é uma coleção com chave de recursos de identidade.
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 60fdb901ecd74f3826604d139cad71d9d0844221
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966755"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="da7fe-103">tipo de recurso identityset</span><span class="sxs-lookup"><span data-stu-id="da7fe-103">identitySet resource type</span></span>

<span data-ttu-id="da7fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da7fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da7fe-105">O recurso **identityset** é uma coleção com chave de recursos de [identidade](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="da7fe-105">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="da7fe-106">É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="da7fe-106">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da7fe-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da7fe-107">JSON representation</span></span>

<span data-ttu-id="da7fe-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da7fe-108">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="da7fe-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da7fe-109">Properties</span></span>

| <span data-ttu-id="da7fe-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da7fe-110">Property</span></span>    | <span data-ttu-id="da7fe-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="da7fe-111">Type</span></span>                    | <span data-ttu-id="da7fe-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="da7fe-112">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="da7fe-113">application</span><span class="sxs-lookup"><span data-stu-id="da7fe-113">application</span></span> | [<span data-ttu-id="da7fe-114">Identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-114">Identity</span></span>](identity.md) | <span data-ttu-id="da7fe-p101">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="da7fe-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="da7fe-117">conversa</span><span class="sxs-lookup"><span data-stu-id="da7fe-117">conversation</span></span>| [<span data-ttu-id="da7fe-118">Identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-118">Identity</span></span>](identity.md) | <span data-ttu-id="da7fe-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="da7fe-119">Optional.</span></span> <span data-ttu-id="da7fe-120">A equipe ou canal associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="da7fe-120">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="da7fe-121">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="da7fe-121">conversationIdentityType</span></span>| [<span data-ttu-id="da7fe-122">Identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-122">Identity</span></span>](identity.md) | <span data-ttu-id="da7fe-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="da7fe-123">Optional.</span></span> <span data-ttu-id="da7fe-124">Indica se a propriedade de **conversa** identifica uma equipe ou um canal.</span><span class="sxs-lookup"><span data-stu-id="da7fe-124">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="da7fe-125">device</span><span class="sxs-lookup"><span data-stu-id="da7fe-125">device</span></span>      | [<span data-ttu-id="da7fe-126">Identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-126">Identity</span></span>](identity.md) | <span data-ttu-id="da7fe-p104">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="da7fe-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="da7fe-129">phone</span><span class="sxs-lookup"><span data-stu-id="da7fe-129">phone</span></span>       | [<span data-ttu-id="da7fe-130">identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-130">identity</span></span>](identity.md) | <span data-ttu-id="da7fe-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="da7fe-131">Optional.</span></span> <span data-ttu-id="da7fe-132">O número de telefone associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="da7fe-132">The phone number associated with this action.</span></span> |
| <span data-ttu-id="da7fe-133">user</span><span class="sxs-lookup"><span data-stu-id="da7fe-133">user</span></span>        | [<span data-ttu-id="da7fe-134">Identity</span><span class="sxs-lookup"><span data-stu-id="da7fe-134">Identity</span></span>](identity.md) | <span data-ttu-id="da7fe-p106">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="da7fe-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="da7fe-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="da7fe-137">Remarks</span></span> 

<span data-ttu-id="da7fe-138">Confira [chamada](call.md) para uso de recursos **identityset** .</span><span class="sxs-lookup"><span data-stu-id="da7fe-138">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


