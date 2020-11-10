---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 951a9e9aa7834f53d1cd9d4e14aaed4b6a2ef71d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969888"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().publications("{id}")
    .buildRequest()
    .delete();

```