---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e003d0d1daffeed590e8e1e75c1b046f3fb0c70e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345330"
---
```powershell

Import-Module Microsoft.Graph.Groups

Get-MgGroupDelta -Property "displayName,description,mailNickname" 

```