---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d07db04f3c41c92b2abbcc190cb0c1b58b5552a4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352388"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePosition -UserId $userId -WorkPositionId $workPositionId

```