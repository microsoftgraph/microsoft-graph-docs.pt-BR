---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c85ece38a37754c55f0d6e8018616b5a76417cc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IMicrosoftAuthenticatorAuthenticationMethodCollectionPage microsoftAuthenticatorMethods = graphClient.users("anirban@contoso.com").authentication().microsoftAuthenticatorMethods()
    .buildRequest()
    .get();

```