---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2030dd0ba575e95c00d470336460b1106335ae2d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980670"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Library Assist";

String description = "Self help community for library";

String mailNickname = "libassist";

EnumSet<ClonableTeamParts> partsToClone = EnumSet.of(ClonableTeamParts.APPS,ClonableTeamParts.TABS,ClonableTeamParts.SETTINGS,ClonableTeamParts.CHANNELS,ClonableTeamParts.MEMBERS);

TeamVisibilityType visibility = TeamVisibilityType.PUBLIC;

graphClient.teams("{id}")
    .clone(TeamCloneParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withDescription(description)
        .withMailNickname(mailNickname)
        .withClassification(null)
        .withVisibility(visibility)
        .withPartsToClone(partsToClone)
        .build())
    .buildRequest()
    .post();

```