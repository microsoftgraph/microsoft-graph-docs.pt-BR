---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9a8c2d1bb61f0300da554d9f37960eb3260f8e8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205178"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.roleManagement().directory().roleAssignmentScheduleRequests("95c690fb-3eb3-4942-a03f-4524aed6f31e")
    .cancel()
    .buildRequest()
    .post();

```