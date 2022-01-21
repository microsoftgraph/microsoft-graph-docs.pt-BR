---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e474b2ddc71e8b0f6287d91ba8c8d39b92931d3e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097984"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AccountEnabled = $false
}

Update-MgDevice -DeviceId $deviceId -BodyParameter $params

```