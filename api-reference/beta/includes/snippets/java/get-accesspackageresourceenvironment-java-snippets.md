---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8d94977a4b41551ebfa309fe1b20a00e954b6e0140217db71802ba5175fbe5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898275"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceEnvironment accessPackageResourceEnvironment = graphClient.identityGovernance().entitlementManagement().accessPackageResourceEnvironments("{accessPackageResourceEnvironmentId}")
    .buildRequest()
    .get();

```