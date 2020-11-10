---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 078179dc01574521f1d9a5e078efde3f119f5048
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961663"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().events("AAMkAGE1M88AADUv0uAAAG=").attachments("AAMkAGE1Mg72tgf7hJp0PICVGCc0g=")
    .buildRequest()
    .get();

```