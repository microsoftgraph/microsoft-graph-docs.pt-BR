---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7357e7ed7eac39651a1c46b6285c1f736b4dea17
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350823"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ReceivedDateTime = [System.DateTime]::Parse("datetime-value")
    SentDateTime = [System.DateTime]::Parse("datetime-value")
    HasAttachments = $true
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    BodyPreview = "bodyPreview-value"
}

# A UPN can also be used as -UserId.
New-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```