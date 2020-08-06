---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 206fbf3ac0763ce5de50f4de40eb12b3f4943081
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567271"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentitySecurityDefaultsEnforcementPolicy identitySecurityDefaultsEnforcementPolicy = graphClient.policies().identitySecurityDefaultsEnforcementPolicy()
    .buildRequest()
    .get();

```