---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd934f3cf6da951a3af0e17f151f7fcffe7d7b49
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097284"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "Display name"
}

New-MgApplication -BodyParameter $params

```