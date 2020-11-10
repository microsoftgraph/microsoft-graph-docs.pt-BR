---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efab098b76613134c8c33d869abcd0bc7fce95cf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972373"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Set set = new Set();
set.description = "mySet";

graphClient.termStore().sets("{setId}")
    .buildRequest()
    .patch(set);

```