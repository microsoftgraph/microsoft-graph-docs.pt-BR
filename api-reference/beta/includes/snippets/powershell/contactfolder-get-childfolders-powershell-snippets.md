---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b68a38ee249fb85825f94b377f7f25a6d0ea1aae
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349577"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContactFolderChildFolder -UserId $userId -ContactFolderId $contactFolderId

```