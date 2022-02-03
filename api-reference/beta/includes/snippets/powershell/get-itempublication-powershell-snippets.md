---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb6349fe047b0b4d2886f797de3e96403e820bfa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351712"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId

```