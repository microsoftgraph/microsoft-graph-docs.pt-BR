---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b853bcd59fe3d17aae2d1f09bf7bc7f901d17b25
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343092"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    SkuId = "6fd2c87f-b296-42f0-b197-1e91e994b900"
    ServicePlanId = "a23b959c-7ce8-4e57-9140-b90eb88a9e97"
}

Initialize-MgOrganizationService -OrganizationId $organizationId -BodyParameter $params

```