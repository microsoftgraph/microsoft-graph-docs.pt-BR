---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3e7e58d95510e0ed8d2f6ec59e476d4ec342079
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971578"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalItem externalItem = new ExternalItem();
LinkedList<Acl> aclList = new LinkedList<Acl>();
Acl acl = new Acl();
acl.type = AclType.EVERYONE;
acl.value = "67a141d8-cf4e-4528-ba07-bed21bfacd2d";
acl.accessType = AccessType.GRANT;
acl.identitySource = "azureActiveDirectory";
aclList.add(acl);
externalItem.acl = aclList;

graphClient.connections("contosohr").items("TSP228082938")
    .buildRequest()
    .patch(externalItem);

```