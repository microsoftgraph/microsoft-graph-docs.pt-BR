---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31e253fe3312869860e5527dc1bda5c913a5a25eaea4c9d8191f40b56b967204
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupLifecyclePolicy groupLifecyclePolicy = new GroupLifecyclePolicy();
groupLifecyclePolicy.groupLifetimeInDays = 100;
groupLifecyclePolicy.managedGroupTypes = "Selected";
groupLifecyclePolicy.alternateNotificationEmails = "admin@contoso.com";

graphClient.groupLifecyclePolicies()
    .buildRequest()
    .post(groupLifecyclePolicy);

```