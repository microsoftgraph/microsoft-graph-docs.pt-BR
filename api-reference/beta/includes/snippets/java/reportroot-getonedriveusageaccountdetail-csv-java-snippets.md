---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9ae9beb7f1a64e8523fd46179eb1ccfa3fbe8fd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872977"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOneDriveUsageAccountDetailCollectionPage getOneDriveUsageAccountDetail = graphClient.reports()
    .getOneDriveUsageAccountDetail('D7')
    .buildRequest()
    .get();

```