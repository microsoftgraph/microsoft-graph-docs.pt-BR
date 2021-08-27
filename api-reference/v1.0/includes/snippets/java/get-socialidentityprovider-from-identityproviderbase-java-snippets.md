---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37fa12ad60630582838aea4bc93e6f35e0a0d2b714eb2f63cde51ba4e47862ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407081"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("Amazon-OAUTH")
    .buildRequest()
    .get();

```