---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39ac514ea4771062b130ce0246ba67491589912a
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910320"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = new TokenLifetimePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenLifetimePolicy.definition = definitionList;
tokenLifetimePolicy.displayName = "displayName-value";
tokenLifetimePolicy.isOrganizationDefault = true;

graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .patch(tokenLifetimePolicy);

```