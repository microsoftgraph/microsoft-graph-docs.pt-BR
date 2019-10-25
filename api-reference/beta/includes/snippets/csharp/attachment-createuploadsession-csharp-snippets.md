---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48dd92fc58e4137efb2eb16eaa5e2ec150f5d925
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37637341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachmentItem = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "flower",
    Size = 3483322
};

await graphClient.Me.Messages["AAMkADI5MAAIT3drCAAA="].Attachments
    .CreateUploadSession(attachmentItem)
    .Request()
    .PostAsync();

```