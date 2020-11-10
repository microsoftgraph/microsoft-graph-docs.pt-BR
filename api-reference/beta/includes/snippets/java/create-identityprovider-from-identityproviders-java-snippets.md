---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92548f7d07463e5919eb8e57e99f77ee35833f08
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953372"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = new IdentityProvider();
identityProvider.name = "Login with Amazon";
identityProvider.type = "Amazon";
identityProvider.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
identityProvider.clientSecret = "000000000000";

graphClient.identityProviders()
    .buildRequest()
    .post(identityProvider);

```