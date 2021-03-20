---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9d531cb44c37dce7812ff7c3a69d50a201cd1e26
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975696"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .get();

```