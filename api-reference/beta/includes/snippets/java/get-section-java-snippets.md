---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88e2d8a8dfe276a610861cde8f252be959cc3a06
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979541"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteSection onenoteSection = graphClient.me().onenote().sections("{id}")
    .buildRequest()
    .get();

```