---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: faae72c20f8bbf65e174a313c8dc1e416694ac7c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344636"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    UserAccountType = "administrator"
}

Rename-MgDeviceManagementVirtualEndpointCloudPcUserAccountType -CloudPCId $cloudPCId -BodyParameter $params

```