---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 787140d9255bcba47c581b0eb9e722194eef521e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873639"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMailboxUsageStorageCollectionPage getMailboxUsageStorage = graphClient.reports()
    .getMailboxUsageStorage('D7')
    .buildRequest()
    .get();

```