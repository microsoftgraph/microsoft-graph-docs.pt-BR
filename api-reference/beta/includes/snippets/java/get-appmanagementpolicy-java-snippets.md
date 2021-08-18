---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9d51c7f5635120c0255fd036999d5fa66c13507
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicy appManagementPolicy = graphClient.policies().appManagementPolicies("{id}")
    .buildRequest()
    .get();

```