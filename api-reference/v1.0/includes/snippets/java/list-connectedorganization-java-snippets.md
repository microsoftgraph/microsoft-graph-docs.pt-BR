---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58a265f16dda9251259895a37829b26a1beb22f1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342444"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganizationCollectionPage connectedOrganizations = graphClient.identityGovernance().entitlementManagement().connectedOrganizations()
    .buildRequest()
    .get();

```