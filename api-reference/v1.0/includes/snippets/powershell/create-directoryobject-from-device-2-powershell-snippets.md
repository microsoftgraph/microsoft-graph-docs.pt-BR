---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9328ca2f33137fa4a9837f73f6f5f1aa6ff9b04
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101218"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgDeviceRegisteredUserByRef -DeviceId $deviceId -BodyParameter $params

```