---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03e547b4a0b552f5eb7fc8a00155f07dac419f30
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758705"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5";
oAuth2PermissionGrant.consentType = "AllPrincipals";
oAuth2PermissionGrant.resourceId = "943603e4-e787-4fe9-93d1-e30f749aae39";
oAuth2PermissionGrant.scope = "DelegatedPermissionGrant.ReadWrite.All";

graphClient.oauth2PermissionGrants()
    .buildRequest()
    .post(oAuth2PermissionGrant);

```