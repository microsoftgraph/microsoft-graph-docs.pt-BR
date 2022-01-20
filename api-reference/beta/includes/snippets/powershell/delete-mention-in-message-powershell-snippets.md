---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2bbb2e8855a47549d1d3c18f3867e91018972689
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133401"
---
```powershell

Import-Module Microsoft.Graph.Mail

Remove-MgUserMessageMention -UserId $userId -MessageId $messageId -MentionId $mentionId

```