---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8a312e19299ed43c7d1162777a2dfe5f12004eb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359466"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessDeviceUsageUserCountsCollectionPage getSkypeForBusinessDeviceUsageUserCounts = graphClient.reports()
    .getSkypeForBusinessDeviceUsageUserCounts("D7")
    .buildRequest()
    .get();

```