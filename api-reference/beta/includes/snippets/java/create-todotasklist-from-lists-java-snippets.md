---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7318fd47ac9f450d7ff69cb03a634ca3d006bded3410a9c85f34272cd9f251b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = new TodoTaskList();
todoTaskList.displayName = "Travel items";

graphClient.me().todo().lists()
    .buildRequest()
    .post(todoTaskList);

```