---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b2af29f8bc38519f757ac54e07390e64d4344e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978334"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .removeKey(ServicePrincipalRemoveKeyParameterSet
        .newBuilder()
        .withKeyId(keyId)
        .withProof(proof)
        .build())
    .buildRequest()
    .post();

```