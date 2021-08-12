---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9381444023b0b9f67107066623efd6d3e1f9a116da237d463c5f0d8dbea8e521
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240401"
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