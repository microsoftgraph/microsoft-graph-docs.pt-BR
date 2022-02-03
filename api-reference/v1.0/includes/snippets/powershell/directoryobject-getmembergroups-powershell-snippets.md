---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8f5f82106e56031f25444e521090a3261af5452
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339507"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    SecurityEnabledOnly = $false
}

Get-MgDirectoryObjectMemberGroup -DirectoryObjectId $directoryObjectId -BodyParameter $params

```