---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec7375aa4f4a582a8246578a169071ca8ab5c945
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2020
ms.locfileid: "45224612"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.devices("{id}").registeredOwners("{id}").reference()
    .buildRequest()
    .delete();

```