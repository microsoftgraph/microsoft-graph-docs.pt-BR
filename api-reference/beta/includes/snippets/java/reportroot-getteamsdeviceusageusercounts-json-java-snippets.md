---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9e475229d8d509c4ff72afbc2ad2b2ea0b78c42
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871806"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITeamsDeviceUsageUserCountsCollectionPage getTeamsDeviceUsageUserCounts = graphClient.reports()
    .getTeamsDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```