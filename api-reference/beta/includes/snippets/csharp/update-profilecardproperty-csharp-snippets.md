---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35298bef31f3a3d1a48b736ad758b4300b08aef1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803525"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var profileCardProperty = new ProfileCardProperty
{
    Annotations = new List<ProfileCardAnnotation>()
    {
        new ProfileCardAnnotation
        {
            Localizations = new List<DisplayNameLocalization>()
            {
                new DisplayNameLocalization
                {
                    LanguageTag = "no-NB",
                    DisplayName = "Kostnads Senter"
                }
            }
        }
    }
};

await graphClient.Organization["{organization-id}"].Settings.ProfileCardProperties["{profileCardProperty-id}"]
    .Request()
    .UpdateAsync(profileCardProperty);

```