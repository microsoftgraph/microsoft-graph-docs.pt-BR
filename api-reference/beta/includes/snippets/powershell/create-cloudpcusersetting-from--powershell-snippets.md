---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba05d0fc90bab5b84d2c30b95f03058853ea86fb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334195"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcUserSetting"
    DisplayName = "Example"
    SelfServiceEnabled = $false
    LocalAdminEnabled = $true
    RestorePointSetting = @{
        FrequencyInHours = 16
        UserRestoreEnabled = $true
    }
}

New-MgDeviceManagementVirtualEndpointUserSetting -BodyParameter $params

```