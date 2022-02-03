---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e6d0f6c0a6281cec3765290c3df821b68a59cad
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350992"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId

```