---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7986467faab5a7382cf2d6fcdef4bb71c2e8fb1a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351055"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "Greater Seattle District Technical Schools"
}

Update-MgAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```