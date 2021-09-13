---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 481990a917ffce2f9c6f5f72cacd3304337ba60eacd2d37fdf93c26f04ec19c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216206"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("{id}").appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```