---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ee6cda65997448dd92b76ed2c2e19c60d22cef3aca5529977985981ea94a420
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328010"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = new Permission();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("read");
permission.roles = rolesList;

graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .patch(permission);

```