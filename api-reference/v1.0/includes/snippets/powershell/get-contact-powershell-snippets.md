---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 590ee4f031ffaa507238eb59d3c4982ff37a3ddd
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350019"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContact -UserId $userId -ContactId $contactId

```