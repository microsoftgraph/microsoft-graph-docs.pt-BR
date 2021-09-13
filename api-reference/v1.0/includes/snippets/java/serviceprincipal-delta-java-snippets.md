---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e71bb86efa6fe39d88cc6070e13f4816497536ad7d075c426b55ef079627a5c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157903"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalDeltaCollectionPage delta = graphClient.servicePrincipals()
    .delta()
    .buildRequest()
    .get();

```