---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02b3dc48a67a0a4aa1c06a66d7d5154dd342b02f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967850"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";

graphClient.serviceprincipals()
    .buildRequest()
    .post(servicePrincipal);

```