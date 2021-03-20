---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2c05ad8c2ef657b254f2aebed1fc6ad0994298c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945058"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrinterShareCollectionPage shares = graphClient.print().shares()
    .buildRequest()
    .get();

```