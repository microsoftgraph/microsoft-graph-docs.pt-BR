---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e13b91267e8f69490a2051101ec00f103074fe0b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128460"
---
```powershell

Import-Module Microsoft.Graph.Reports

Get-MgAuditLogSignIn -Filter "startsWith(appDisplayName,'Graph')" -Top 10 

```