---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63de6b1749eedc56b3ddc8ccdd49cd6841e99f3a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334942"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.displayName = "Access Package New Name";

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .buildRequest()
    .patch(accessPackage);

```