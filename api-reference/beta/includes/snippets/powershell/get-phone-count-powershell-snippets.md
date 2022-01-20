---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76ed84b6d47d5d8000cd120d96fd432b4f93c590
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112774"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgContact -Search "displayName:wa" -CountVariable CountVar -ConsistencyLevel eventual 


```