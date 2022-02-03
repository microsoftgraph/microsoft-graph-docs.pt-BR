---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd516cf6fd710e33c82d06adfc6ffbf6089a1dc4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341466"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    DisplayName = "Myprefix_test_mysuffix"
    MailNickname = "Myprefix_test_mysuffix"
    OnBehalfOfUserId = "onBehalfOfUserId-value"
}

Test-MgGroupProperty -GroupId $groupId -BodyParameter $params

```