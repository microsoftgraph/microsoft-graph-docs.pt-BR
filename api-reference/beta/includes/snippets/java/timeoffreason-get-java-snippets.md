---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f5ee5768d5ba1f8d32594e85e80c111a071b068
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867995"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOffReason timeOffReason = graphClient.teams("{teamId}").schedule().timeOffReasons("{timeOffReasonId}")
    .buildRequest()
    .get();

```