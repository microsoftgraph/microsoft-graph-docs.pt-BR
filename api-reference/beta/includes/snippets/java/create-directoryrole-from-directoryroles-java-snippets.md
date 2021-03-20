---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d02ca657f731bd437f4b66b09b4d9b00f23140b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975852"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = new DirectoryRole();
directoryRole.description = "description-value";
directoryRole.displayName = "displayName-value";
directoryRole.roleTemplateId = "roleTemplateId-value";

graphClient.directoryRoles()
    .buildRequest()
    .post(directoryRole);

```