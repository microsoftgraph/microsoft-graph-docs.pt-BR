---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70c8e05b2ce245e301891495d67ddad24563022c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981191"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkAGUzY5QKjAAA=").attachments("AAMkAGUzY5QKjAAABEgAQAMkpJI_X-LBFgvrv1PlZYd8=")
    .buildRequest()
    .get();

```