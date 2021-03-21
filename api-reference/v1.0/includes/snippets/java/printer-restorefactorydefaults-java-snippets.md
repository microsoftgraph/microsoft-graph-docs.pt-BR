---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7849fb53ed38cf8b74455df60c8714daff14370c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969259"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```