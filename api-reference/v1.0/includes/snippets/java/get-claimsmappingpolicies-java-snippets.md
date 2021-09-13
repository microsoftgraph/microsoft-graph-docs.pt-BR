---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ce19551e799b87b49ba259bbc521ec7d6c26fc362b5235ec9f8c5dc39b96bae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327579"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ClaimsMappingPolicyCollectionPage claimsMappingPolicies = graphClient.policies().claimsMappingPolicies()
    .buildRequest()
    .get();

```