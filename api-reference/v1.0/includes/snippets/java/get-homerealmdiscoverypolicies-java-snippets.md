---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72785a9aba06b514a7e79eb5b90ef111a43ab561
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50983261"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicyCollectionPage homeRealmDiscoveryPolicies = graphClient.policies().homeRealmDiscoveryPolicies()
    .buildRequest()
    .get();

```