---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 526c7439bf3ca94b64a53d38f83916b7c84f28f16a06c25955defb6d01f2b6d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlowCollectionPage b2cUserFlows = graphClient.identity().b2cUserFlows()
    .buildRequest()
    .expand("identityProviders")
    .get();

```