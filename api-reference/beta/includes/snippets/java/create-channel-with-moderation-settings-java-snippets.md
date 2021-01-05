---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1069f2212df952510580831b8c9ba02927ec094
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753784"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.displayName = "TestChannelModeration";
channel.description = "Test channel moderation.";
channel.membershipType = ChannelMembershipType.STANDARD;
ChannelModerationSettings moderationSettings = new ChannelModerationSettings();
moderationSettings.userNewMessageRestriction = UserNewMessageRestriction.EVERYONE_EXCEPT_GUESTS;
moderationSettings.replyRestriction = ReplyRestriction.EVERYONE;
moderationSettings.allowNewMessageFromBots = true;
moderationSettings.allowNewMessageFromConnectors = true;
channel.moderationSettings = moderationSettings;

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels()
    .buildRequest()
    .post(channel);

```