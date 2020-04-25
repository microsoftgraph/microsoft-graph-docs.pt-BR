---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 75f4761429ee3de2c7ba9c21efb89b9d39e851d5
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805471"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
homeRealmDiscoveryPolicy.definition = definitionList;
homeRealmDiscoveryPolicy.displayName = "displayName-value";
homeRealmDiscoveryPolicy.isOrganizationDefault = true;
homeRealmDiscoveryPolicy.type = "type-value";

graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .patch(homeRealmDiscoveryPolicy);

```