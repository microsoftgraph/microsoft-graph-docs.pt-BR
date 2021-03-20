---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9cc652dfb8352024d20d24bbc9a123e32a0ff05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967621"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();
identityApiConnector.displayName = "New Test API";
identityApiConnector.targetUrl = "https://otherapi.com/api/endpoint";
BasicAuthentication authenticationConfiguration = new BasicAuthentication();
authenticationConfiguration.username = "<NEW_USERNAME>";
authenticationConfiguration.password = "<NEW_PASSWORD>";
identityApiConnector.authenticationConfiguration = authenticationConfiguration;

graphClient.identity().apiConnectors("{identityApiConnectorId}")
    .buildRequest()
    .patch(identityApiConnector);

```