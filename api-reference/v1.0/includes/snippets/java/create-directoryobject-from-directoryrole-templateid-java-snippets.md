---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6315a142c934b9a05d509bcbf5e7490292f256cd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522641"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = new DirectoryObject();
directoryObject.id = "{user-id}";

graphClient.directoryRoles("roleTemplateId={role-templateId}").members().references()
    .buildRequest()
    .post(directoryObject);

```