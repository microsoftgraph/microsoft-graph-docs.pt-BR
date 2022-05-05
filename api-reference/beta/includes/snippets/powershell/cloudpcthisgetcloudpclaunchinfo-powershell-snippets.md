---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dba894081fc03286de12a7152f9b6bea0eb60115
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209325"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserCloudPcLaunchInfo -UserId $userId -CloudPCId $cloudPCId

```