---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 350470ecdfae1dd21c42f2f58323a1a6499971bb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348660"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserContactFolderContactDelta -UserId $userId -ContactFolderId $contactFolderId -Property "displayName" 

```