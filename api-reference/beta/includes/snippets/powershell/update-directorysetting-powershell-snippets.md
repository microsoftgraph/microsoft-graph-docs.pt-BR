---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d8c886f8240669936357ef1c139bdbb485a44ef
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410531"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Values = @(
        @{
            Name = "CustomBlockedWordsList"
            Value = "Contoso"
        }
    )
}

Update-MgDirectorySetting -DirectorySettingId $directorySettingId -BodyParameter $params

```