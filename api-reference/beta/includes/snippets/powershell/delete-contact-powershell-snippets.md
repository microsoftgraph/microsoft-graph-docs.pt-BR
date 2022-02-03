---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33725b0e905648da329944ed16080979936d47dd
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349762"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Remove-MgUserContact -UserId $userId -ContactId $contactId

```