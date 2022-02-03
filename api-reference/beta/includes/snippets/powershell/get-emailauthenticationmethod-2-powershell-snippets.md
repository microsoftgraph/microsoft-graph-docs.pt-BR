---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cea4aaa3a53a52fa6a7c8e02ff823d66b1a8473
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350796"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationEmailMethod -UserId $userId

```