---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02e84b94ed5232d458785b81cfea462a5b393f5a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkAGUzY5QKgAAA=").attachments("AAMkAGUzY5QKgAAABEgAQAISJOe1FEqdNsMEQmpZjRW8=")
    .buildRequest()
    .get();

```