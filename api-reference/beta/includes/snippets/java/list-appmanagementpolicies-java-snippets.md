---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb313347d507109268270400b24ab821945e2c60
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258921"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppManagementPolicyCollectionPage appManagementPolicies = graphClient.policies().appManagementPolicies()
    .buildRequest()
    .get();

```