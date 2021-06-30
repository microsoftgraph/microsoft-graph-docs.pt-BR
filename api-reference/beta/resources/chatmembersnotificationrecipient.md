---
title: tipo de recurso chatMembersNotificationRecipient
description: Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade. O destinatário consiste nos membros do chat.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3743d9d37e934cd61f699febfcc148afb8e84e98
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211210"
---
# <a name="chatmembersnotificationrecipient-resource-type"></a><span data-ttu-id="23636-104">tipo de recurso chatMembersNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="23636-104">chatMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="23636-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23636-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23636-106">Representa o destinatário de uma notificação enviada em um feed Microsoft Teams atividade.</span><span class="sxs-lookup"><span data-stu-id="23636-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="23636-107">O destinatário consiste nos membros do chat.</span><span class="sxs-lookup"><span data-stu-id="23636-107">The recipient consists of the chat members.</span></span>

<span data-ttu-id="23636-108">Herda de [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="23636-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="23636-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23636-109">Properties</span></span>
|<span data-ttu-id="23636-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23636-110">Property</span></span>|<span data-ttu-id="23636-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="23636-111">Type</span></span>|<span data-ttu-id="23636-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="23636-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23636-113">chatId</span><span class="sxs-lookup"><span data-stu-id="23636-113">chatId</span></span>|<span data-ttu-id="23636-114">String</span><span class="sxs-lookup"><span data-stu-id="23636-114">String</span></span>|<span data-ttu-id="23636-115">O identificador do chat.</span><span class="sxs-lookup"><span data-stu-id="23636-115">The chat's identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23636-116">Relações</span><span class="sxs-lookup"><span data-stu-id="23636-116">Relationships</span></span>
<span data-ttu-id="23636-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23636-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23636-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23636-118">JSON representation</span></span>
<span data-ttu-id="23636-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23636-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.chatMembersNotificationRecipient",
  "chatId": "String"
}
```

