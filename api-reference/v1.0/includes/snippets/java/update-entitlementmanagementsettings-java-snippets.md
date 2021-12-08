---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e13b9d8cb4e751ac67641f5f00c1e3b524fe88e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336886"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EntitlementManagementSettings entitlementManagementSettings = new EntitlementManagementSettings();
entitlementManagementSettings.externalUserLifecycleAction = AccessPackageExternalUserLifecycleAction.NONE;

graphClient.identityGovernance().entitlementManagement().settings()
    .buildRequest()
    .patch(entitlementManagementSettings);

```