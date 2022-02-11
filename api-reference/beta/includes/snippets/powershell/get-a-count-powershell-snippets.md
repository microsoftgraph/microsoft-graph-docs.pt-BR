---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c131cb70abe6c707e7a3e98751ad926b4980d13
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530529"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContact -Filter "startswith(displayName,'A')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```