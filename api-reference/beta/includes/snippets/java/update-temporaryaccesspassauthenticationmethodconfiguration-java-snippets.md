---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dad9131d3692ea9ee1e90f2f7cdfbed6ce06db1c236d4e73115daeb1b3334023
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099495"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TemporaryAccessPassAuthenticationMethodConfiguration authenticationMethodConfiguration = new TemporaryAccessPassAuthenticationMethodConfiguration();
authenticationMethodConfiguration.state = AuthenticationMethodState.ENABLED;
authenticationMethodConfiguration.defaultLifetimeInMinutes = 60;
authenticationMethodConfiguration.defaultLength = 8;
authenticationMethodConfiguration.minimumLifetimeInMinutes = 60;
authenticationMethodConfiguration.maximumLifetimeInMinutes = 1440;
authenticationMethodConfiguration.
  isUsableOnce = false;
LinkedList<AuthenticationMethodTarget> includeTargetsList = new LinkedList<AuthenticationMethodTarget>();
AuthenticationMethodTarget includeTargets = new AuthenticationMethodTarget();
includeTargets.targetType = AuthenticationMethodTargetType.GROUP;
includeTargets.id = "all_users";
includeTargets.isRegistrationRequired = false;
includeTargets.useForSignIn = true;
includeTargetsList.add(includeTargets);
AuthenticationMethodTargetCollectionResponse authenticationMethodTargetCollectionResponse = new AuthenticationMethodTargetCollectionResponse();
authenticationMethodTargetCollectionResponse.value = includeTargetsList;
AuthenticationMethodTargetCollectionPage authenticationMethodTargetCollectionPage = new AuthenticationMethodTargetCollectionPage(authenticationMethodTargetCollectionResponse, null);
authenticationMethodConfiguration.includeTargets = authenticationMethodTargetCollectionPage;

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("TemporaryAccessPass")
    .buildRequest()
    .patch(authenticationMethodConfiguration);

```