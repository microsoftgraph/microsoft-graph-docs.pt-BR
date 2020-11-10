---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87b94260c9bd9f5f7b972353879fafaebde78c8c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48978630"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").rows("{index}")
    .range()
    .buildRequest()
    .post();

```