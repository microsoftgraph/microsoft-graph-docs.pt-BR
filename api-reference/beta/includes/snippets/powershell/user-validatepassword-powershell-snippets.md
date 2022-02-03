---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad2d067620062a30ed6943c8d328d99b56e7d84b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340914"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Password = "1234567890"
}

Test-MgUserPassword -BodyParameter $params

```