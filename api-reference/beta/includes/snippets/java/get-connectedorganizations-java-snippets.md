---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58a265f16dda9251259895a37829b26a1beb22f1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganizationCollectionPage connectedOrganizations = graphClient.identityGovernance().entitlementManagement().connectedOrganizations()
    .buildRequest()
    .get();

```