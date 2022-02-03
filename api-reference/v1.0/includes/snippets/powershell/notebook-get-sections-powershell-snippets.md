---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7907e672b97842353a2f9eb62efde6d2c677a567
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349455"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebookSection -UserId $userId -NotebookId $notebookId

```