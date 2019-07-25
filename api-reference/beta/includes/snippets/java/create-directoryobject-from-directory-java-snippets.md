---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2324d06d50333b00b3587e9dffa04acef43d5009
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862536"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .restore()
    .buildRequest()
    .post();

```