---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73a2db60a81ba7cb15e02cc70575a43b50568b2f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347268"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().connectedOrganizations("{connectedOrganizationId}")
    .buildRequest()
    .delete();

```