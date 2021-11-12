---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c02200277005e059d8f91bbe43a71f00b01816e51cf006f7c9090958561d5cde
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900021"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReferenceAttachment attachment = new ReferenceAttachment();
attachment.name = "Personal pictures";
attachment.sourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics";
attachment.providerType = ReferenceAttachmentProvider.ONE_DRIVE_CONSUMER;
attachment.permission = ReferenceAttachmentPermission.EDIT;
attachment.isFolder = false;

graphClient.me().messages("AAMkAGE1M88AADUv0uFAAA=").attachments()
    .buildRequest()
    .post(attachment);

```