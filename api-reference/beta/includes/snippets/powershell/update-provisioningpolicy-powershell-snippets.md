---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a827bc355ae71680c4db70f752057d51059ec116
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131440"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    DisplayName = "HR provisioning policy"
    Description = "Provisioning policy for India HR employees"
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701b553"
}

Update-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -BodyParameter $params

```