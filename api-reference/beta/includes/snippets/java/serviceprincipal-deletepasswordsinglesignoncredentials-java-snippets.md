---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5670d787b2f8cf9dfccc72009256157549bc5c5eb8b0c264f6a616990bbee2c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215543"
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