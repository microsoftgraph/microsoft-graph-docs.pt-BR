---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c6cfe782c53a8fb3aa8d4f69d4e0026c067eef3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106674"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -ExpandProperty "assignments" 

```