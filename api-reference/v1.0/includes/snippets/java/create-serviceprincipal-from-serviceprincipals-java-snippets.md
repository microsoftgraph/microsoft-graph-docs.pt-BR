---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e96326ae29a88b4e7d2e2ff6ee3f7c3725686cb8
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905368"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";

graphClient.servicePrincipals()
    .buildRequest()
    .post(servicePrincipal);

```