---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d321ff522b0cb71cfcd65b2d5b1cbad68847536f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100287"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Values = @(
        @{
            Name = "name-value"
            Value = "value-value"
        }
    )
}

Update-MgDirectorySetting -DirectorySettingId $directorySettingId -BodyParameter $params

```