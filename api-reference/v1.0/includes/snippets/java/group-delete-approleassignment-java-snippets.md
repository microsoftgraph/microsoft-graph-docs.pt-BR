---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 369194cfb2edc5eb8a30a601a9df7ebb84593651
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978816"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```