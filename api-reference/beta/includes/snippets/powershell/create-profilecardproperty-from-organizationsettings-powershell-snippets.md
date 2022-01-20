---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b789675581981438d0034e6537541825a52b4c26
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112800"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DirectoryPropertyName = "CustomAttribute1"
    Annotations = @(
        @{
            DisplayName = "Cost Center"
            Localizations = @(
                @{
                    LanguageTag = "ru-RU"
                    DisplayName = "центр затрат"
                }
            )
        }
    )
}

New-MgOrganizationSettingProfileCardProperty -OrganizationId $organizationId -BodyParameter $params

```