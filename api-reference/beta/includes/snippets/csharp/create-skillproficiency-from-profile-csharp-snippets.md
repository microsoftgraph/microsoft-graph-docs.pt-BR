---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fb7a623404fd470dac031be85ce0a671ae3b245eeb333559d4251d0a6edf8dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214601"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "Professional"
    },
    AllowedAudiences = AllowedAudiences.Organization,
    DisplayName = "API Design",
    Proficiency = SkillProficiencyLevel.GeneralProfessional,
    CollaborationTags = new List<String>()
    {
        "ableToMentor"
    }
};

await graphClient.Me.Profile.Skills
    .Request()
    .AddAsync(skillProficiency);

```