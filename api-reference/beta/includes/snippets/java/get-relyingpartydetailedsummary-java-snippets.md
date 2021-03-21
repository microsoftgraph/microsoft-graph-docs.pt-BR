---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17fd183fb74aae64432d698c7d75afc876877550
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetRelyingPartyDetailedSummaryCollectionPage getRelyingPartyDetailedSummary = graphClient.reports()
    .getRelyingPartyDetailedSummary(ReportRootGetRelyingPartyDetailedSummaryParameterSet
        .newBuilder()
        .withPeriod("period_value")
        .build())
    .buildRequest()
    .get();

```