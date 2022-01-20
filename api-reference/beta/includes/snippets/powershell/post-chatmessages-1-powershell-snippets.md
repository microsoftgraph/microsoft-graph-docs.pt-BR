---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 119943db37e1d7c80d7a9c6d94ea8d3b5fa48eec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116335"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        Content = "Hello world"
    }
}

New-MgChatMessage -ChatId $chatId -BodyParameter $params

```