---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3ad4d66bbd4a1dfc89782b61487726955df682c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475072"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().temporaryAccessPassMethods("{id}")
    .buildRequest()
    .delete();

```