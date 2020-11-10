---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee6f0e012bd3c242d07675ca862b103a6b5014b5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969908"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = graphClient.me().profile().patents("{id}")
    .buildRequest()
    .get();

```