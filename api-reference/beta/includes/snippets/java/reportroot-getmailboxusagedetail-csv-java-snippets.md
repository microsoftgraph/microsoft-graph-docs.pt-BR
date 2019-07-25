---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a3e0c1f06e59b2cccfba79748538aa174166335
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873775"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageDetailCollectionPage getMailboxUsageDetail = graphClient.reports()
    .getMailboxUsageDetail('D7')
    .buildRequest()
    .get();

```