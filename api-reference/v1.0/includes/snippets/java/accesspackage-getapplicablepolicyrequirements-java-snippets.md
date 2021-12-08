---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81aeec114c913f2fb461b7267687410dcfab3a5b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334911"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .getApplicablePolicyRequirements()
    .buildRequest()
    .post();

```