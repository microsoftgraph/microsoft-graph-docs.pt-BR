---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da6e6c802330fe03fca0c5fdc4c31559a29be8f6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972436"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = graphClient.print().printers("{id}")
    .buildRequest()
    .get();

```