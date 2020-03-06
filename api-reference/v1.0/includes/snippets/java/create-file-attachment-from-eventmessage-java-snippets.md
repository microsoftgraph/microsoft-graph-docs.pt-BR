---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a192d2f661abf51533c5a66f706d41a679a07fc9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FileAttachment attachment = new FileAttachment();
attachment.name = "name-value";
attachment.contentType = "contentType-value";
attachment.isInline = false;
attachment.contentLocation = "contentLocation-value";
attachment.contentBytes = "base64-contentBytes-value";

graphClient.me().messages("{id}").attachments()
    .buildRequest()
    .post(attachment);

```