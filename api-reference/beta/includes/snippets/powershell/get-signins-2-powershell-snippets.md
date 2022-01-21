---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7c810a5ca979c54224b46586b402161ac7c934d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095910"
---
```powershell

Import-Module Microsoft.Graph.Reports

Get-MgAuditLogSignIn -Filter "startsWith(appDisplayName,'Azure')" -Top 10 

```