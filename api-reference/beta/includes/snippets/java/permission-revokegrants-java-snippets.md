---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4e401f3a2cda301909d49ebfe3baae645d9ff6eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977895"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> granteesList = new LinkedList<DriveRecipient>();
DriveRecipient grantees = new DriveRecipient();
grantees.email = "ryan@contoso.com";

granteesList.add(grantees);

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .revokeGrants(PermissionRevokeGrantsParameterSet
        .newBuilder()
        .withGrantees(granteesList)
        .build())
    .buildRequest()
    .post();

```