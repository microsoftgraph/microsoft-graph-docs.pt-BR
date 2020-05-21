---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02b3dc48a67a0a4aa1c06a66d7d5154dd342b02f
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335838"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";

graphClient.serviceprincipals()
    .buildRequest()
    .post(servicePrincipal);

```