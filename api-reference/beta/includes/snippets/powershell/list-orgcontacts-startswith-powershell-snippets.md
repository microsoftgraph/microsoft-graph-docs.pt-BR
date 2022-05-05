---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c131cb70abe6c707e7a3e98751ad926b4980d13
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203259"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContact -Filter "startswith(displayName,'A')" -CountVariable CountVar -Top 1 -Sort "displayName" -ConsistencyLevel eventual 


```