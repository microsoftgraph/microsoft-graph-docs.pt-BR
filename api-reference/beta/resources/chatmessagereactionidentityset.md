---
title: Tipo de recurso chatMessageReactionIdentitySet
description: Representa um usuário que reagia a uma mensagem em um chat ou canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 032b335656d768f505cdb673b56ef0955cf9ed58
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211195"
---
# <a name="chatmessagereactionidentityset-resource-type"></a><span data-ttu-id="55c7b-103">Tipo de recurso chatMessageReactionIdentitySet</span><span class="sxs-lookup"><span data-stu-id="55c7b-103">chatMessageReactionIdentitySet resource type</span></span>

<span data-ttu-id="55c7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55c7b-105">Representa um **usuário** que reagia a [uma mensagem](../resources/chatmessage.md) em um chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="55c7b-105">Represents a **user** that reacted to a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="55c7b-106">Somente a `user` propriedade tem um valor.</span><span class="sxs-lookup"><span data-stu-id="55c7b-106">Only the `user` property has a value.</span></span>


<span data-ttu-id="55c7b-107">Herda de [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="55c7b-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="55c7b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55c7b-108">Properties</span></span>
|<span data-ttu-id="55c7b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55c7b-109">Property</span></span>|<span data-ttu-id="55c7b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="55c7b-110">Type</span></span>|<span data-ttu-id="55c7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55c7b-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="55c7b-112">application</span></span>|[<span data-ttu-id="55c7b-113">identity</span><span class="sxs-lookup"><span data-stu-id="55c7b-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="55c7b-114">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="55c7b-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="55c7b-115">Não definido porque os aplicativos não podem reagir às mensagens.</span><span class="sxs-lookup"><span data-stu-id="55c7b-115">Not set because applications can't react to messages.</span></span>|
|<span data-ttu-id="55c7b-116">device</span><span class="sxs-lookup"><span data-stu-id="55c7b-116">device</span></span>|[<span data-ttu-id="55c7b-117">identity</span><span class="sxs-lookup"><span data-stu-id="55c7b-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="55c7b-118">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="55c7b-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="55c7b-119">Não definido porque os dispositivos não podem reagir às mensagens.</span><span class="sxs-lookup"><span data-stu-id="55c7b-119">Not set because devices can't react to messages.</span></span>|
|<span data-ttu-id="55c7b-120">user</span><span class="sxs-lookup"><span data-stu-id="55c7b-120">user</span></span>|[<span data-ttu-id="55c7b-121">identity</span><span class="sxs-lookup"><span data-stu-id="55c7b-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="55c7b-122">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="55c7b-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="55c7b-123">Detalhes sobre o usuário que reagia à mensagem.</span><span class="sxs-lookup"><span data-stu-id="55c7b-123">Details about the user who reacted to the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55c7b-124">Relações</span><span class="sxs-lookup"><span data-stu-id="55c7b-124">Relationships</span></span>
<span data-ttu-id="55c7b-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55c7b-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55c7b-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55c7b-126">JSON representation</span></span>
<span data-ttu-id="55c7b-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55c7b-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageReactionIdentitySet",
  "user": {
    "@odata.type": "microsoft.graph.identity"
  },
  "application": {
    "@odata.type": "microsoft.graph.identity"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity"
  }
}
```

