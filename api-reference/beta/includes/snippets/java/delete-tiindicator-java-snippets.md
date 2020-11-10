---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87b76a757f6a82385c3bb51b84df037884c439aa
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977769"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .delete();

```