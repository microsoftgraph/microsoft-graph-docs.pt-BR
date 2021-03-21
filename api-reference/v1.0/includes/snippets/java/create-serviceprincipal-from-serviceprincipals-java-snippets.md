---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18a3e5c7ac9d7270c89bab4cd8fee0d6f01d0027
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";

graphClient.servicePrincipals()
    .buildRequest()
    .post(servicePrincipal);

```