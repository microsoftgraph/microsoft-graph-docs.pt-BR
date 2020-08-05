---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08d09e5ca0cb8f5e30e60fc89b17ef43aa05e262
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567379"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AttachmentItem attachmentItem = new AttachmentItem();
attachmentItem.attachmentType = AttachmentType.FILE;
attachmentItem.name = "flower";
attachmentItem.size = 3483322;

graphClient.me().events("AAMkADU5CCmSAAA=").attachments()
    .createUploadSession(attachmentItem)
    .buildRequest()
    .post();

```