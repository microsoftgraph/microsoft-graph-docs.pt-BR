---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69051688de9238e32b6ad602f5ad7423cb20d2cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973916"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreatePrivateChannels = true;
memberSettings.allowCreateUpdateChannels = true;
team.memberSettings = memberSettings;
TeamMessagingSettings messagingSettings = new TeamMessagingSettings();
messagingSettings.allowUserEditMessages = true;
messagingSettings.allowUserDeleteMessages = true;
team.messagingSettings = messagingSettings;
TeamFunSettings funSettings = new TeamFunSettings();
funSettings.allowGiphy = true;
funSettings.giphyContentRating = GiphyRatingType.STRICT;
team.funSettings = funSettings;

graphClient.groups("{id}").team()
    .buildRequest()
    .put(team);

```