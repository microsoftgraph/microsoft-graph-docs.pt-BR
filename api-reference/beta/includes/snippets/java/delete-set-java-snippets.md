---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 600fcee50018483f0bab198e58eff68a496b2641
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980079"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.termStore().sets("{setId}")
    .buildRequest()
    .delete();

```