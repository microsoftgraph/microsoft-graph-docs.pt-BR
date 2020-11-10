---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d466ec4da8b8b2b5e37f3bd838c061e22a031a7c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979758"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{id}")
    .buildRequest()
    .delete();

```