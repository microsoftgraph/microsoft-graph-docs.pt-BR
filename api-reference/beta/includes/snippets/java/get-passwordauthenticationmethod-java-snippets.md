---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0895963ad13b2f2a604f9e3517d87662ba22fece
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973052"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordAuthenticationMethod passwordAuthenticationMethod = graphClient.me().authentication().passwordMethods("{id}")
    .buildRequest()
    .get();

```