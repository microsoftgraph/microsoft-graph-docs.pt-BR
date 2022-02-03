---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce8b0c4418e71d253af0f7f355b7a10a47493080
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352415"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "Section name"
}

# A UPN can also be used as -UserId.
New-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId -BodyParameter $params

```