---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31fa80260aa03447bd483f8042e1be58af61d34f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969627"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetCredentialUsageSummaryCollectionPage getCredentialUsageSummary = graphClient.reports()
    .getCredentialUsageSummary(ReportRootGetCredentialUsageSummaryParameterSet
        .newBuilder()
        .withPeriod("D30")
        .build())
    .buildRequest()
    .filter("feature eq 'registration'")
    .get();

```