---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0341321102de784b1781f238c4955565c215850
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976368"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetAzureADApplicationSignInSummaryCollectionPage getAzureADApplicationSignInSummary = graphClient.reports()
    .getAzureADApplicationSignInSummary(ReportRootGetAzureADApplicationSignInSummaryParameterSet
        .newBuilder()
        .withPeriod("D7")
        .build())
    .buildRequest()
    .get();

```