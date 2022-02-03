---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74c0ebd22a5320d8de6cc9488973eb078932b35d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351676"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

# A UPN can also be used as -UserId.
Get-MgUserScopedRoleMemberOf -UserId $userId

```