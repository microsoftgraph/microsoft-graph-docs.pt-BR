---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 028dddde8ed4374a2141c91eb66030df5a1aaaa6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124351"
---
```powershell

Import-Module Microsoft.Graph.Applications

Get-MgApplication -Search "displayName:Web" -CountVariable CountVar -ConsistencyLevel eventual 


```