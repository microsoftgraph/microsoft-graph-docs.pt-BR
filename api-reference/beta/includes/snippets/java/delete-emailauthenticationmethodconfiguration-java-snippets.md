---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3db2b16f95ad1ca2139651fe7a0ed417e073be27
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472959"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .delete();

```