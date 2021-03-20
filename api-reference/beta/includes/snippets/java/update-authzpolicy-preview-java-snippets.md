---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5d487249ebb0cf35d0da63edb963eb589daa2e4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977132"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthorizationPolicy authorizationPolicy = new AuthorizationPolicy();
LinkedList<String> enabledPreviewFeaturesList = new LinkedList<String>();
enabledPreviewFeaturesList.add("assignGroupsToRoles");
authorizationPolicy.enabledPreviewFeatures = enabledPreviewFeaturesList;

graphClient.policies().authorizationPolicy("authorizationPolicy")
    .buildRequest()
    .patch(authorizationPolicy);

```