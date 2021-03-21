---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a12c4d798ded192812778fcd88814aea0ed99372
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968881"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .get();

```