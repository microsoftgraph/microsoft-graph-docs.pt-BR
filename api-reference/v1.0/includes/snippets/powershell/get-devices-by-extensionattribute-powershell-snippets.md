---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbf3a2cd320ce06b3faa7e36c337cf7a72f52134
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62225502"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDevice -Filter "extensionAttributes/extensionAttribute1 eq 'BYOD-Device'" -CountVariable CountVar -ConsistencyLevel eventual 


```