---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5788077d365ffa1e7d1dc95e68f989fb4724fc5d
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522642"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{user-id}";

graphClient.directoryRoles("{role-objectId}").members().references()
    .buildRequest()
    .post(directoryObject);

```