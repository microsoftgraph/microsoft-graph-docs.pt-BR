---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9c29586dccbf24c19812c29a4868b6322c5da06fdfb03e360daab5d4be3268c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272756"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SocialIdentityProvider identityProviderBase = new SocialIdentityProvider();
identityProviderBase.clientSecret = "1111111111111";

graphClient.identity().identityProviders("Amazon-OAUTH")
    .buildRequest()
    .patch(identityProviderBase);

```