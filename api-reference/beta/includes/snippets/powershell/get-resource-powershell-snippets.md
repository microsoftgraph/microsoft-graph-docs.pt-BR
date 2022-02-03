---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3071be91fbb45ac810859bd129726ef62f4cdcd3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351485"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteResourceContent -UserId $userId -OnenoteResourceId $onenoteResourceId

```