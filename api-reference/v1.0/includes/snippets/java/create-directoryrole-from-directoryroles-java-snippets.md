---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d036ad32f6ef72a5e3f9e9275fac35592b8d5f2e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = new DirectoryRole();
directoryRole.roleTemplateId = "roleTemplateId-value";

graphClient.directoryRoles()
    .buildRequest()
    .post(directoryRole);

```