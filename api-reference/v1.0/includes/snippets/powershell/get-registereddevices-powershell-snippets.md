---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3fd0f3d0c4afadad376465a589e3b4a81c47543
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350566"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserRegisteredDevice -UserId $userId

```