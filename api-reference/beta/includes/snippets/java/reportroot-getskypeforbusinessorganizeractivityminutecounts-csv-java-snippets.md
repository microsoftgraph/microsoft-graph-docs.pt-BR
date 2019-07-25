---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8d8e58b5192912c7f1a85236f6734c76a608eba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35872177"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessOrganizerActivityMinuteCountsCollectionPage getSkypeForBusinessOrganizerActivityMinuteCounts = graphClient.reports()
    .getSkypeForBusinessOrganizerActivityMinuteCounts('D7')
    .buildRequest()
    .get();

```