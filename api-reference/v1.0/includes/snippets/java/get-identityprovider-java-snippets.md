---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f58dd040ee1411e321609ad30e53278d7a21e96
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979504"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = graphClient.identityProviders("Amazon-OAuth")
    .buildRequest()
    .get();

```