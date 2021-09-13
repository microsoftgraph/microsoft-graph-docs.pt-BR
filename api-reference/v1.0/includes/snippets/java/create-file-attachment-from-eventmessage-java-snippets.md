---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c31083f4c8aca7b25b21e49e041bb5a5120084d8e4f68eff8b03ab7f2db8eea9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101540"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = Base64.getDecoder().decode("base64-contentBytes-value");

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```