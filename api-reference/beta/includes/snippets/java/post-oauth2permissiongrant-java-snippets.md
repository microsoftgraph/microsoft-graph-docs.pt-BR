---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f30a4f84cab6e9450b9558011a0de965340da19
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48967535"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "clientId-value";
oAuth2PermissionGrant.consentType = "consentType-value";
oAuth2PermissionGrant.principalId = "principalId-value";
oAuth2PermissionGrant.resourceId = "resourceId-value";
oAuth2PermissionGrant.scope = "scope-value";
oAuth2PermissionGrant.startTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
oAuth2PermissionGrant.expiryTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");

graphClient.oauth2PermissionGrants()
    .buildRequest()
    .post(oAuth2PermissionGrant);

```