---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b88be8c1375ef68ad061211ad83d141ac49a8095
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352207"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId

```