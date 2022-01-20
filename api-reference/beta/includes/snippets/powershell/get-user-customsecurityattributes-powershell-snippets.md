---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57bcabb1357ee3c672af25e9faeb4414422b99a6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119795"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUser -UserId $userId -Property "customSecurityAttributes" 

```