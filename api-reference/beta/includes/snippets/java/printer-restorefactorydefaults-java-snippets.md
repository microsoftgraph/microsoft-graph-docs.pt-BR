---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee4f587ab4f933833443fad62d34ea56ec1c29d3
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979786"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{id}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```