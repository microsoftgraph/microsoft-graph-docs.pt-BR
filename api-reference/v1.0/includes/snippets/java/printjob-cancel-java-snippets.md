---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c16dfd2fd72e8d9dc8fb68302fd193667a1861a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777072"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .cancel()
    .buildRequest()
    .post();

```