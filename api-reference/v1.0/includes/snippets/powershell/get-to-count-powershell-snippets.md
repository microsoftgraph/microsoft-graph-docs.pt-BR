---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1528c92f0e21c1d1e31928aab4815b14563909b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100777"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Search "displayName:wa" OR "displayName:ad" -Orderbydisplayname =  -CountVariable CountVar -ConsistencyLevel eventual 


```