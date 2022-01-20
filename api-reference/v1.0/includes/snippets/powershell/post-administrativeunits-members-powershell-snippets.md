---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5cb2db8794e5329f7afd7fe4e9ce9bd886bda580
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092644"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/groups/{id}"
}

New-MgDirectoryAdministrativeUnitMemberByRef -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```