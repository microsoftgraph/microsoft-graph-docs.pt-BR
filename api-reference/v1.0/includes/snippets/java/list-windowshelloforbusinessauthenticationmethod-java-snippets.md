---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1b562ec4d64a81786233da058827e0e02334080b76d05b35736a3218e084008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102372"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsHelloForBusinessAuthenticationMethodCollectionPage windowsHelloForBusinessMethods = graphClient.users("annie@contoso.com").authentication().windowsHelloForBusinessMethods()
    .buildRequest()
    .get();

```