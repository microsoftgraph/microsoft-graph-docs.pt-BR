---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 733e8e69a2a0878eecd28d11fd51132a39aef32f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350549"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOwnedDevice -UserId $userId

```