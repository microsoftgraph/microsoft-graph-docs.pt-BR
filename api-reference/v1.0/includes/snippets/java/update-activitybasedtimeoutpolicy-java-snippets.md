---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a92b3e0a26961eec0f16913b1e6c0cc20138e5e9aad7c8a50b47ddde3cf9bcea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159016"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ActivityBasedTimeoutPolicy activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
activityBasedTimeoutPolicy.definition = definitionList;
activityBasedTimeoutPolicy.displayName = "displayName-value";
activityBasedTimeoutPolicy.isOrganizationDefault = true;

graphClient.policies().activityBasedTimeoutPolicies("{id}")
    .buildRequest()
    .patch(activityBasedTimeoutPolicy);

```