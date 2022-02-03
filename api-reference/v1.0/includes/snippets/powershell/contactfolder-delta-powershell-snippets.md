---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e59923f7d689dc5ea756111b335d8d566bdd7295
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342369"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserContactFolderDelta -UserId $userId

```