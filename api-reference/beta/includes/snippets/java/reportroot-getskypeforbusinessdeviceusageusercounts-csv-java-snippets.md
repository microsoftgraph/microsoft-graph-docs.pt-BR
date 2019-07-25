---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6304b88066df0a8d1a64c3cf2bd0a2752d87611b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872277"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageUserCountsCollectionPage getSkypeForBusinessDeviceUsageUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserCounts('D7')
    .buildRequest()
    .get();

```