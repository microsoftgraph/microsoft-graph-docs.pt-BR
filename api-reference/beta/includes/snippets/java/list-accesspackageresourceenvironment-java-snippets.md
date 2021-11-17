---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4f3399b13bbe48b62f3c189451af827ac29fe1462937ca94bb3e55135711f4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898273"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceEnvironmentCollectionPage accessPackageResourceEnvironments = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments()
    .buildRequest()
    .filter("originSystem eq 'SharePointOnline'")
    .get();

```