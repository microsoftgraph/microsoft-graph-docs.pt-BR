---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fd5ba24a5aecf99671ee0e20e68ce093db99616048ca26518227e8844ec34a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214599"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SkillProficiency skillProficiency = new SkillProficiency();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Professional");
skillProficiency.categories = categoriesList;
skillProficiency.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);
skillProficiency.displayName = "API Design";
skillProficiency.proficiency = SkillProficiencyLevel.GENERAL_PROFESSIONAL;
LinkedList<String> collaborationTagsList = new LinkedList<String>();
collaborationTagsList.add("ableToMentor");
skillProficiency.collaborationTags = collaborationTagsList;

graphClient.me().profile().skills()
    .buildRequest()
    .post(skillProficiency);

```