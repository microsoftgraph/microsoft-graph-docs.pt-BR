---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c48375dcd227b6c13aced45a397820701f62eb4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980065"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkAGUzY5QKgAAA=").attachments("AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=")
    .buildRequest()
    .get();

```