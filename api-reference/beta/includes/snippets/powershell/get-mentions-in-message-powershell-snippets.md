---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1c83f6ef866f51a7821b32723b46450ecd3609a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099501"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "mentions" 

```