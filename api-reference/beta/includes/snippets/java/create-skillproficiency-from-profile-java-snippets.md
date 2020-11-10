---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c82316303ea8619604054b94ad6071247bb63d64
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972716"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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