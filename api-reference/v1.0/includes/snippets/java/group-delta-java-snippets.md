---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49a8516ed82d085dfc2fbefe80847b8c238fa4e0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890805"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupDeltaCollectionPage delta = graphClient.groups()
    .delta()
    .buildRequest()
    .get();

```