---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3713a5c1efb65f9e4fe553751be873194dcb7ce557b550f45677b1aa935e5ad2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329254"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var skillProficiency = new SkillProficiency
{
    Categories = new List<String>()
    {
        "Professional"
    },
    Proficiency = SkillProficiencyLevel.AdvancedProfessional
};

await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .UpdateAsync(skillProficiency);

```