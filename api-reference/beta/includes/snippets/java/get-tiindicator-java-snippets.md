---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8f2556bbe5f7af94fb15495ab7abdea1cb87b64
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977706"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = graphClient.security().tiIndicators("{id}")
    .buildRequest()
    .get();

```