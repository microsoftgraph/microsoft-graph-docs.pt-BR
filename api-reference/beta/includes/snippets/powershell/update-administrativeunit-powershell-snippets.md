---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99f9ca4a3ed290cd2a004c5b2226ac1df08aba7d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097382"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "displayName-value"
    Description = "description-value"
    Visibility = "visibility-value"
}

Update-MgAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```