---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d1ca3c127631babbdb03ce336a22ab439b910f93e7ffee6994c30ee43e9e50f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376832"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = new DirectoryRole();
directoryRole.roleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1";

graphClient.directoryRoles()
    .buildRequest()
    .post(directoryRole);

```