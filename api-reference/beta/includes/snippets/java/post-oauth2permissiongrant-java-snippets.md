---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60fbe82169ae41344ccf3a5492368551a7cb41cf456830f187515f682398c27d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099651"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "clientId-value";
oAuth2PermissionGrant.consentType = "consentType-value";
oAuth2PermissionGrant.principalId = "principalId-value";
oAuth2PermissionGrant.resourceId = "resourceId-value";
oAuth2PermissionGrant.scope = "scope-value";
oAuth2PermissionGrant.startTime = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");
oAuth2PermissionGrant.expiryTime = OffsetDateTimeSerializer.deserialize("2016-10-19T10:37:00Z");

graphClient.oauth2PermissionGrants()
    .buildRequest()
    .post(oAuth2PermissionGrant);

```