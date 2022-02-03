---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77bd9810eed26a2e4c806d909a40dcb34e140bd8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339492"
---
```powershell

Import-Module Microsoft.Graph.DirectoryObjects

$params = @{
    SecurityEnabledOnly = $true
}

Get-MgDirectoryObjectMemberObject -DirectoryObjectId $directoryObjectId -BodyParameter $params

```