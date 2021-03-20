---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb820c2d79d17ee5834b3c7a66171bc094c17958
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975844"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .delete();

```