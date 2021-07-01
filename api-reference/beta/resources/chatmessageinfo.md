---
title: Tipo de recurso chatMessageInfo
description: Representa uma visualização de um recurso chatMessage.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dc03ee6743aa8115f5a231b3766cc2d6c3d5537b
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236286"
---
# <a name="chatmessageinfo-resource-type"></a><span data-ttu-id="e1cdd-103">Tipo de recurso chatMessageInfo</span><span class="sxs-lookup"><span data-stu-id="e1cdd-103">chatMessageInfo resource type</span></span>

<span data-ttu-id="e1cdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1cdd-105">Representa uma visualização de um [recurso chatMessage.](../resources/chatmessage.md)</span><span class="sxs-lookup"><span data-stu-id="e1cdd-105">Represents a preview of a [chatMessage](../resources/chatmessage.md) resource.</span></span> <span data-ttu-id="e1cdd-106">Esse objeto só pode ser buscado como parte de uma lista de [chats](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="e1cdd-106">This object can only be fetched as part of a list of [chats](../resources/chat.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1cdd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1cdd-107">Properties</span></span>
|<span data-ttu-id="e1cdd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1cdd-108">Property</span></span>|<span data-ttu-id="e1cdd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1cdd-109">Type</span></span>|<span data-ttu-id="e1cdd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1cdd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cdd-111">corpo</span><span class="sxs-lookup"><span data-stu-id="e1cdd-111">body</span></span>|[<span data-ttu-id="e1cdd-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="e1cdd-112">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="e1cdd-113">Corpo do [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e1cdd-113">Body of the [chatMessage](../resources/chatmessage.md).</span></span> <span data-ttu-id="e1cdd-114">Isso ainda conterá marcadores para @mentions e anexos, mesmo que o objeto não retorne @mentions e anexos.</span><span class="sxs-lookup"><span data-stu-id="e1cdd-114">This will still contain markers for @mentions and attachments even though the object does not return @mentions and attachments.</span></span>|
|<span data-ttu-id="e1cdd-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1cdd-115">createdDateTime</span></span>|<span data-ttu-id="e1cdd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1cdd-116">DateTimeOffset</span></span>|<span data-ttu-id="e1cdd-117">Objeto date time representando a hora em que a mensagem foi criada.</span><span class="sxs-lookup"><span data-stu-id="e1cdd-117">Date time object representing the time at which message was created.</span></span>|
|<span data-ttu-id="e1cdd-118">from</span><span class="sxs-lookup"><span data-stu-id="e1cdd-118">from</span></span>|[<span data-ttu-id="e1cdd-119">chatMessageFromIdentitySet</span><span class="sxs-lookup"><span data-stu-id="e1cdd-119">chatMessageFromIdentitySet</span></span>](../resources/chatmessagefromidentityset.md)|<span data-ttu-id="e1cdd-120">Informações sobre o remetente da mensagem.</span><span class="sxs-lookup"><span data-stu-id="e1cdd-120">Information about the sender of the message.</span></span>|
|<span data-ttu-id="e1cdd-121">id</span><span class="sxs-lookup"><span data-stu-id="e1cdd-121">id</span></span>|<span data-ttu-id="e1cdd-122">String</span><span class="sxs-lookup"><span data-stu-id="e1cdd-122">String</span></span>|<span data-ttu-id="e1cdd-123">ID do [chatMessage](../resources/chatmessage.md).</span><span class="sxs-lookup"><span data-stu-id="e1cdd-123">ID of the [chatMessage](../resources/chatmessage.md).</span></span>|
|<span data-ttu-id="e1cdd-124">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e1cdd-124">isDeleted</span></span>|<span data-ttu-id="e1cdd-125">Booleano</span><span class="sxs-lookup"><span data-stu-id="e1cdd-125">Boolean</span></span>|<span data-ttu-id="e1cdd-126">Se definido como `true` , a mensagem original foi excluída.</span><span class="sxs-lookup"><span data-stu-id="e1cdd-126">If set to `true`, the original message has been deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1cdd-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e1cdd-127">Relationships</span></span>
<span data-ttu-id="e1cdd-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1cdd-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1cdd-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1cdd-129">JSON representation</span></span>
<span data-ttu-id="e1cdd-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1cdd-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageInfo",
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "from": {
    "@odata.type": "microsoft.graph.chatMessageFromIdentitySet"
  },
  "createdDateTime": "String (timestamp)",
  "isDeleted": "Boolean"
}
```

## <a name="see-also"></a><span data-ttu-id="e1cdd-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1cdd-131">See also</span></span>

- [<span data-ttu-id="e1cdd-132">chat</span><span class="sxs-lookup"><span data-stu-id="e1cdd-132">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="e1cdd-133">chatMessage</span><span class="sxs-lookup"><span data-stu-id="e1cdd-133">chatMessage</span></span>](../resources/chatmessage.md)

