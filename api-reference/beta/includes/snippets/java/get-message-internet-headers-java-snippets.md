---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18f7eb13b44820bdd011cbb7a6e61a5c91eda92c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979862"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkAGVmMDEz")
    .buildRequest()
    .select("internetMessageHeaders")
    .get();

```