---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 281837bcbb34ecb5b799ad9af62a31a03de480bb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347113"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Post = @{
        Body = @{
            ContentType = "text"
            Content = "I attached a reference to a file on OneDrive."
        }
        Attachments = @(
            @{
                "@odata.type" = "#microsoft.graph.referenceAttachment"
                Name = "Personal pictures"
                SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
                ProviderType = "oneDriveConsumer"
                Permission = "Edit"
                IsFolder = "True"
            }
        )
    }
}

Invoke-MgReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```