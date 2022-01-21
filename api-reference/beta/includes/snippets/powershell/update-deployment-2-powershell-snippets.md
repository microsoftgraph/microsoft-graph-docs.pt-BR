---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 984ef2dc2ab7decb5d89a406430553c39e908526
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095607"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    "@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
    Settings = @{
        "@odata.type" = "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
        Monitoring = @{
            MonitoringRules = @(
                @{
                    Signal = "rollback"
                    Threshold = 5
                    Action = "pauseDeployment"
                }
            )
        }
    }
}

Update-MgWindowsUpdatesDeployment -DeploymentId $deploymentId -BodyParameter $params

```