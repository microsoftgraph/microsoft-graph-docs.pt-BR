---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09dae5390d94d8b2d479b716ff092ff7882d649d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872373"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageDistributionUserCountsCollectionPage getSkypeForBusinessDeviceUsageDistributionUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageDistributionUserCounts('D7')
    .buildRequest()
    .get();

```