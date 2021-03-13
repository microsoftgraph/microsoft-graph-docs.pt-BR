---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 401cffd5ee944a5732541b6307b19d36a283cb8c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775994"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJob printJob = graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .buildRequest()
    .get();

```