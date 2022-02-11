---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f457b1ed6de6f67e7db259cacfaee44c926119db
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530542"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    RelatedContacts = @(
        @{
            DisplayName = "Father Time"
            EmailAddress = "father@time.com"
            MobilePhone = "4251231234"
            Relationship = "guardian"
            AccessConsent = $true
        }
        @{
            DisplayName = "Mother Nature"
            EmailAddress = "mother@nature.co.uk"
            MobilePhone = "3251231234"
            Relationship = "parent"
            AccessConsent = $true
        }
    )
}

Update-MgEducationUser -EducationUserId $educationUserId -BodyParameter $params

```