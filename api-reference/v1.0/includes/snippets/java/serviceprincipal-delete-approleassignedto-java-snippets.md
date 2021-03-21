---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62572b792722edff5caa6e5f358376b3944c8d8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958196"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").appRoleAssignedTo("{id}")
    .buildRequest()
    .delete();

```