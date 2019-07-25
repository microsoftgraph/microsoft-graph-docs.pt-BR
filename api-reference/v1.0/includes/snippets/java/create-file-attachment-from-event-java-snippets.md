---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c41ebcf19366617493184b2df85cc823348c2694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887276"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = new Attachment();
attachment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.fileAttachment"));
attachment.name = "menu.txt";
attachment.contentBytes = "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=";

graphClient.me().events("AAMkAGI1AAAt9AHjAAA=").attachments()
    .buildRequest()
    .post(attachment);

```