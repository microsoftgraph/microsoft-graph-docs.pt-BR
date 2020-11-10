---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9169ed2044da5d6a4e1e359169b64088e85912a5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977909"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Program program = new Program();
program.displayName = "testprogram3";
program.description = "test description";

graphClient.programs()
    .buildRequest()
    .post(program);

```