---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 966ae92434036b5c38472576e0d7e508d614154b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475801"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITemporaryAccessPassAuthenticationMethodCollectionPage temporaryAccessPassMethods = graphClient.me().authentication().temporaryAccessPassMethods()
    .buildRequest()
    .get();

```