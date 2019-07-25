---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 185ab99cb5c91c01cbacb3fb79d156fc5d78098e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869803"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Shift shift = graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .get();

```