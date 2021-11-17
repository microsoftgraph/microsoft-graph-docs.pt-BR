---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf7fa6b8a151dc456d4a730b4bdef95f0f63d87958fb6f6982021c2c25ed58b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215194"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicy claimsMappingPolicy = graphClient.policies().claimsMappingPolicies("{id}")
    .buildRequest()
    .get();

```