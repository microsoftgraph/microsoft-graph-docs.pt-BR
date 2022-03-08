---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61a263fb93da1084850dd66d1056b0fda194d197
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338181"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    CloudPcSnapshotId = "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8"
}

Restore-MgDeviceManagementManagedDeviceCloudPc -ManagedDeviceId $managedDeviceId -BodyParameter $params

```