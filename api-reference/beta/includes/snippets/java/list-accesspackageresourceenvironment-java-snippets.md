---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5def248612362a121d173e3305e9a9cfbc57d38
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978908"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceEnvironmentCollectionPage accessPackageResourceEnvironments = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments()
    .buildRequest()
    .filter("originSystem eq 'SharePointOnline'")
    .get();

```