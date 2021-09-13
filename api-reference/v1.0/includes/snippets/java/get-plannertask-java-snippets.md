---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 246ee7bcd4fce498a0e4b43d9ac599274dd71c71ee784316d077d68a835127c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327893"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerTask plannerTask = graphClient.planner().tasks("{task-id}")
    .buildRequest()
    .get();

```