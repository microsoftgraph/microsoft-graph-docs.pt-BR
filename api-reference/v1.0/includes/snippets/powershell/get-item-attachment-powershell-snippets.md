---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 690dd30f902b89a7f0b5a5896559591d6e27a2ec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136440"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageAttachment -UserId $userId -MessageId $messageId -AttachmentId $attachmentId

```