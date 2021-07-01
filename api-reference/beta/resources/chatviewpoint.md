---
title: Tipo de recurso chatViewpoint
description: Representa propriedades específicas do usuário de um chat.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca6a542903aae7b203c6183a25dd99889b97f275
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236289"
---
# <a name="chatviewpoint-resource-type"></a><span data-ttu-id="c9c22-103">Tipo de recurso chatViewpoint</span><span class="sxs-lookup"><span data-stu-id="c9c22-103">chatViewpoint resource type</span></span>

<span data-ttu-id="c9c22-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c22-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c22-105">Representa propriedades específicas do usuário de um [chat](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="c9c22-105">Represents user-specific properties of a [chat](../resources/chat.md).</span></span> <span data-ttu-id="c9c22-106">Essas propriedades podem mudar com base em quem é o chamador da API.</span><span class="sxs-lookup"><span data-stu-id="c9c22-106">These properties might change based on who the caller of the API is.</span></span>

> <span data-ttu-id="c9c22-107">**Observação:** Atualmente, somente a operação [de chats de lista](../api/chat-list.md) suporta **chatViewpoint**.</span><span class="sxs-lookup"><span data-stu-id="c9c22-107">**Note:** Currently, only the [list chats](../api/chat-list.md) operation supports **chatViewpoint**.</span></span>

## <a name="properties"></a><span data-ttu-id="c9c22-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9c22-108">Properties</span></span>
|<span data-ttu-id="c9c22-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9c22-109">Property</span></span>|<span data-ttu-id="c9c22-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9c22-110">Type</span></span>|<span data-ttu-id="c9c22-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9c22-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9c22-112">lastMessageReadDateTime</span><span class="sxs-lookup"><span data-stu-id="c9c22-112">lastMessageReadDateTime</span></span>|<span data-ttu-id="c9c22-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9c22-113">DateTimeOffset</span></span>|<span data-ttu-id="c9c22-114">Representa a dateTime up até a qual o usuário de chamada leu [chatMessages](../resources/chatmessage.md) em um chat específico.</span><span class="sxs-lookup"><span data-stu-id="c9c22-114">Represents the dateTime up until which the calling user has read [chatMessages](../resources/chatmessage.md) in a specific chat.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9c22-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c9c22-115">Relationships</span></span>
<span data-ttu-id="c9c22-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9c22-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9c22-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9c22-117">JSON representation</span></span>
<span data-ttu-id="c9c22-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9c22-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatViewpoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatViewpoint",
  "lastMessageReadDateTime": "String (timestamp)"
}
```

