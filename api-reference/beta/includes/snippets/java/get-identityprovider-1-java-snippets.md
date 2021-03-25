---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4db70c5801a27a233ab3e64bd5723caea4609561
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210463"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProvider identityProvider = graphClient.identityProviders("{id}")
    .buildRequest()
    .get();

```