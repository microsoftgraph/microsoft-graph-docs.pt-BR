---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36711756326ce77268e2ecda0d924ec686a7079333797e4278cf1d30e150ac0e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTaskCollectionPage tasks = graphClient.planner().buckets("{bucket-id}").tasks()
    .buildRequest()
    .get();

```