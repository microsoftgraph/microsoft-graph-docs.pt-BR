---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce29b4b038f688a9958e02f2a98f3f173461688b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092769"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    ParentFolderId = "AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=="
    DisplayName = "Important contacts"
}

New-MgUserContactFolder -UserId $userId -BodyParameter $params

```