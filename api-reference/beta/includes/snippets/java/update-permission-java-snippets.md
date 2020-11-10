---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 161a0a2b032ba6c31ace951218ba41e1953e70f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973891"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Permission permission = new Permission();
LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("read");
permission.roles = rolesList;

graphClient.me().drive().items("{item-id}").permissions("{perm-id}")
    .buildRequest()
    .patch(permission);

```