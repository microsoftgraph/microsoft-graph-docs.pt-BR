---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 561f1838471ddc31a07dff7e51c65bf8c4ca0ffa551f485f6a68ac5325991d2a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213809"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = Base64.getDecoder().decode("contentBytes-value");

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```