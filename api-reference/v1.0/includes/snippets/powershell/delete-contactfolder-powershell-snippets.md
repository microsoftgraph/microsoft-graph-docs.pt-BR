---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b497a7f0282ea92547bc40a653c5cedad7e49242
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350675"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Remove-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId

```