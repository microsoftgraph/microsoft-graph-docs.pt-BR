---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfecf53d2b8154cc4dfd03bba119ee8f56b779b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971720"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/identity/apiConnectors/{id}"));

graphClient.identity().b2cUserFlows("B2C_1_testuserflow").postFederationSignup().reference()
    .buildRequest()
    .put(identityApiConnector);

```