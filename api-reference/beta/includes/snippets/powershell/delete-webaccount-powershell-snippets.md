---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15258cda67d3aec36c7ee113410d93b46657e91c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351235"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId

```