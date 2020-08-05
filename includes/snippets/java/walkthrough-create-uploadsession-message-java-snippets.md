---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e49dfadc6b753a4c34122adc622f0478a5d53428
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567377"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322;

graphClient.me().messages("AAMkADI5MAAIT3drCAAA=").attachments()
    .createUploadSession(attachmentItem)
    .buildRequest()
    .post();

```