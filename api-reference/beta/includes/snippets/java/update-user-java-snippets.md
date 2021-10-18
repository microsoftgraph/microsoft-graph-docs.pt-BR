---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0d1acb82d5216478db55f12c863e141cb9bc1b522655f85b15111df21f8be30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329310"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("+1 425 555 0109");
user.businessPhones = businessPhonesList;
user.officeLocation = "18/2111";

graphClient.me()
    .buildRequest()
    .patch(user);

```