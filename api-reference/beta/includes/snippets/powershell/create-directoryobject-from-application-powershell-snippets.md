---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a37d2547f78d8a8c14776b90fb417217f70235d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114347"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

New-MgApplicationOwnerByRef -ApplicationId $applicationId -BodyParameter $params

```