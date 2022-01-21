---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11981cd5990605099fc3cd8ff0646107eace62f0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125002"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    DisplayName = "displayName-value"
    Description = "description-value"
    Visibility = "visibility-value"
}

Update-MgDirectoryAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```