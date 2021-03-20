---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d99090c1cd63a002681e2dd00eda88a72ed2ae1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953930"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffRequest timeOffRequest = graphClient.teams("{teamId}").schedule().timeOffRequests("{timeOffRequestId}")
    .buildRequest()
    .get();

```