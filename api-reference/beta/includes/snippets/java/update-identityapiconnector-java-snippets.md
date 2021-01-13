---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28677cc98f05cc52f975eb08c023b287fa5284a9
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844330"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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