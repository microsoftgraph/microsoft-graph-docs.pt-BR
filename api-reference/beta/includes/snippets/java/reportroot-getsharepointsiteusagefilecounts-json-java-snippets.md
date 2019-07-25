---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2e8994350132067edd686f44af1254b371c37596
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872641"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISharePointSiteUsageFileCountsCollectionPage getSharePointSiteUsageFileCounts = graphClient.reports()
    .getSharePointSiteUsageFileCounts('D7')
    .buildRequest()
    .get();

```