---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 672db53feb295826946770db492775d024442d72
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112715"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    BusinessPhones = @(
        "businessPhones-value"
    )
    City = "city-value"
    CompanyName = "companyName-value"
    Country = "country-value"
    Department = "department-value"
    DisplayName = "displayName-value"
}

Update-MgContact -OrgContactId $orgContactId -BodyParameter $params

```