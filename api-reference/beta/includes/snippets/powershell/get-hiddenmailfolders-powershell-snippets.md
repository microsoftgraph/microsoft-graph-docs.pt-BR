---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38825eb85f6a98e3000237097832addacbec41a6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092916"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolder -UserId $userId -Includehiddenfolders true 

```