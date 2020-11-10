---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edbea9bc3db7ff1d42cb23060a1811cb74a3400a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955344"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .buildRequest()
    .delete();

```