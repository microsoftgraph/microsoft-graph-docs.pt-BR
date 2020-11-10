---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00809d7d5b1c6c74b6ad3217e97fbb7f22ef8da6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965367"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .addFavorite()
    .buildRequest()
    .post();

```