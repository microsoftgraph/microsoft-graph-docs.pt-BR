---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49a5297f291e1666d144bbd7f6f745d793ddcfd5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122769"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -Property "subject,body,bodyPreview,uniqueBody" 

```