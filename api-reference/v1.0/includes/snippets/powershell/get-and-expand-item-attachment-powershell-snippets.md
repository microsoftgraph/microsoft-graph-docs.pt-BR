---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6a571a67260536f3ad5fd7d36aa870fb4953279e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136439"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMessageAttachment -UserId $userId -MessageId $messageId -AttachmentId $attachmentId -ExpandProperty "microsoft.graph.itemattachment/item" 

```