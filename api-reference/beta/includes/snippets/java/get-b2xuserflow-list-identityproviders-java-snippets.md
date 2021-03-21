---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71be43d9fc37679ba8c0a6f31dc21c1544aba1f4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981728"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderCollectionWithReferencesPage identityProviders = graphClient.identity().b2xUserFlows("{id}").identityProviders()
    .buildRequest()
    .get();

```