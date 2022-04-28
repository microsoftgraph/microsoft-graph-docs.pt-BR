---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 226ea21a8c7e8d0391ddaf137d02bf5359c1114c72a82b8f9ba9babe26e66bbe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271886"
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