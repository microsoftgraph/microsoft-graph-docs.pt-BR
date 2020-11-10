---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0553579938dee551c83645755a97282aa9047da0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964604"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUsedInsightCollectionPage used = graphClient.me().insights().used()
    .buildRequest()
    .get();

```