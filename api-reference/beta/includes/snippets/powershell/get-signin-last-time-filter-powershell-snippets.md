---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57e72efedabb0272ad427409e10437f207cc56fb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126633"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -Filter "startswith(displayName,'Eric')" -Property "displayName,signInActivity" 

```