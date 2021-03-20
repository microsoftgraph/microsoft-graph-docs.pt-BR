---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6011bbae7afce57e9b9c2200342019dd8c03cc2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "5793aa3b-cca9-4794-679a240f8b58";

graphClient.servicePrincipals("{id}")
    .deletePasswordSingleSignOnCredentials(ServicePrincipalDeletePasswordSingleSignOnCredentialsParameterSet
        .newBuilder()
        .withId(id)
        .build())
    .buildRequest()
    .post();

```