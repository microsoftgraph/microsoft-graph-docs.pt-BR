---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a02df957738ae7f3eaa474a46cf6d6ac78224b28b98a72f214d3d42c23de3feb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
TeamMemberSettings memberSettings = new TeamMemberSettings();
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
TeamDiscoverySettings discoverySettings = new TeamDiscoverySettings();
discoverySettings.showInTeamsSearchAndSuggestions = true;
team.discoverySettings = discoverySettings;

graphClient.groups("{id}").team()
    .buildRequest()
    .put(team);

```