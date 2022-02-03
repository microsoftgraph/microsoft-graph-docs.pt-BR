---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75a9dec9df128627980c8c12e0deb142882f1527
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349641"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicyCollectionWithReferencesPage homeRealmDiscoveryPolicies = graphClient.servicePrincipals("19c308f2-e088-464d-8ccb-7137b7bab660").homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```