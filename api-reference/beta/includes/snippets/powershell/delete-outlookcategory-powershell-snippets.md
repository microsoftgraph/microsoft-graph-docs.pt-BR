---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbc1a5db8f4947c021cfde710106e8cc5a3d3fff
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350292"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Remove-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId

```