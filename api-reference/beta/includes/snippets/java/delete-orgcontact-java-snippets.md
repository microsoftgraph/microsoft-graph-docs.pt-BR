---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45c54efc5004aab3c2877be2fc54f1c840282242
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972113"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.contacts("{id}")
    .buildRequest()
    .delete();

```