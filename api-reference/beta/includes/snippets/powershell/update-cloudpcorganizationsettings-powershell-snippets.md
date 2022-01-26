---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6795f8af5f18448aa9bfd5186daa3cb7abad67c
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224998"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcOrganizationSettings"
    UserAccountType = "standardUser"
    OsVersion = "windows11"
}

Update-MgDeviceManagementVirtualEndpointOrganizationSetting -BodyParameter $params

```