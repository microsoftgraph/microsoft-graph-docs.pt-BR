---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ae28e6d743534b11ba24b7a621bd25c3101dca37ebed8561d773b96d1d160d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240397"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachmentItem = new AttachmentItem
{
    AttachmentType = AttachmentType.File,
    Name = "flower",
    Size = 3483322
};

await graphClient.Me.Events["AAMkADU5CCmSAAA="].Attachments
    .CreateUploadSession(attachmentItem)
    .Request()
    .PostAsync();

```