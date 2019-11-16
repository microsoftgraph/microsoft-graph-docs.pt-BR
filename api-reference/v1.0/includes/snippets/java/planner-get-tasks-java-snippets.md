---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b090b7fa4274d96357f2b97b874548d6d0ad5704
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637943"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerTaskCollectionPage tasks = graphClient.planner().tasks()
    .buildRequest()
    .get();

```