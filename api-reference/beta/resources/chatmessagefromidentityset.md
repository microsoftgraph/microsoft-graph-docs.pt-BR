---
title: Tipo de recurso chatMessageFromIdentitySet
description: Representa o remetente de uma mensagem em um chat ou canal.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6f200e5dcaf3c722dc3e185fc1e12946f7ad1151
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211185"
---
# <a name="chatmessagefromidentityset-resource-type"></a><span data-ttu-id="7f3fc-103">Tipo de recurso chatMessageFromIdentitySet</span><span class="sxs-lookup"><span data-stu-id="7f3fc-103">chatMessageFromIdentitySet resource type</span></span>

<span data-ttu-id="7f3fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f3fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f3fc-105">Representa o remetente de uma [mensagem em](../resources/chatmessage.md) um chat ou canal.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-105">Represents the sender of a [message](../resources/chatmessage.md) in a chat or a channel.</span></span> <span data-ttu-id="7f3fc-106">Esse objeto pode ser para uma mensagem que foi excluída ou enviada pelo sistema Microsoft Teams interno; por exemplo, mensagens de evento para adição `null` de membros.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-106">This object may be `null` for a message that has been deleted or sent by the Microsoft Teams internal system; for example, event messages for addition of members.</span></span>


<span data-ttu-id="7f3fc-107">Herda de [identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="7f3fc-107">Inherits from [identitySet](../resources/identityset.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7f3fc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f3fc-108">Properties</span></span>
|<span data-ttu-id="7f3fc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f3fc-109">Property</span></span>|<span data-ttu-id="7f3fc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f3fc-110">Type</span></span>|<span data-ttu-id="7f3fc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f3fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f3fc-112">aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f3fc-112">application</span></span>|[<span data-ttu-id="7f3fc-113">identity</span><span class="sxs-lookup"><span data-stu-id="7f3fc-113">identity</span></span>](../resources/identity.md)|<span data-ttu-id="7f3fc-114">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="7f3fc-114">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="7f3fc-115">Se presente, representa o aplicativo (por exemplo, bot) que enviou a mensagem.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-115">If present, represents the application (for example, bot) that sent the message.</span></span>|
|<span data-ttu-id="7f3fc-116">device</span><span class="sxs-lookup"><span data-stu-id="7f3fc-116">device</span></span>|[<span data-ttu-id="7f3fc-117">identity</span><span class="sxs-lookup"><span data-stu-id="7f3fc-117">identity</span></span>](../resources/identity.md)|<span data-ttu-id="7f3fc-118">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="7f3fc-118">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="7f3fc-119">Não usado.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-119">Not used.</span></span>|
|<span data-ttu-id="7f3fc-120">user</span><span class="sxs-lookup"><span data-stu-id="7f3fc-120">user</span></span>|[<span data-ttu-id="7f3fc-121">identity</span><span class="sxs-lookup"><span data-stu-id="7f3fc-121">identity</span></span>](../resources/identity.md)|<span data-ttu-id="7f3fc-122">Herdado [de identitySet](../resources/identityset.md).</span><span class="sxs-lookup"><span data-stu-id="7f3fc-122">Inherited from [identitySet](../resources/identityset.md).</span></span> <span data-ttu-id="7f3fc-123">Se presente, representa o usuário que enviou a mensagem.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-123">If present, represents the user that sent the message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f3fc-124">Relações</span><span class="sxs-lookup"><span data-stu-id="7f3fc-124">Relationships</span></span>
<span data-ttu-id="7f3fc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f3fc-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f3fc-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f3fc-126">JSON representation</span></span>
<span data-ttu-id="7f3fc-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f3fc-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageFromIdentitySet",
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

