---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73b1553ac41cfc1cb51895f709f269bafb21ef3d
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870742"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetGroupArchivedPrintJobsCollectionPage getGroupArchivedPrintJobs = graphClient.print().reports()
    .getGroupArchivedPrintJobs(ReportRootGetGroupArchivedPrintJobsParameterSet
        .newBuilder()
        .withGroupId("016b5565-3bbf-4067-b9ff-4d68167eb1a6")
        .withStartDateTime("2021-05-24")
        .withEndDateTime("2021-05-25")
        .build())
    .buildRequest()
    .get();

```