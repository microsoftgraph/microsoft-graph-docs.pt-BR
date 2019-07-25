---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acbd3c83f89dc699f67581289a6f66db77cfcbcb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("10002")
    .buildRequest()
    .delete();

```