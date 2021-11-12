---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2becc4751bce39d7cbedc3759aa8c7fb3e56e4e9081a6f34a2a89151bc98679d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160304"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerAssignedToTaskBoardTaskFormat plannerAssignedToTaskBoardTaskFormat = graphClient.planner().tasks("01gzSlKkIUSUl6DF_EilrmQAKDhh").assignedToTaskBoardFormat()
    .buildRequest()
    .get();

```