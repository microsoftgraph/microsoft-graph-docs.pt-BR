---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3fe434104be098c951e504f39052d17151aecc0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129593"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

Get-MgPrivilegedRoleRoleAssignment -Filter "isElevated eq true and expirationDateTime ne null or isElevated eq false" 

```