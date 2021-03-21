---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbff260239ca5d7bd36e6a3ba4d5a32df95622a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me()
    .revokeSignInSessions()
    .buildRequest()
    .post();

```