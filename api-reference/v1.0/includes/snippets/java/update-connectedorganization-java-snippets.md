---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb5c3f2da5b951f2c07f41041ee3e378a2d80afc
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346704"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectedOrganization connectedOrganization = new ConnectedOrganization();
connectedOrganization.displayName = "Connected organization new name";
connectedOrganization.description = "Connected organization new description";
connectedOrganization.state = ConnectedOrganizationState.CONFIGURED;

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{id}")
    .buildRequest()
    .patch(connectedOrganization);

```