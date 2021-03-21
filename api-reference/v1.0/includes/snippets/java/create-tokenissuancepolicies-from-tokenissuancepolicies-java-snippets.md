---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1c93cdeef42b414d8d2e6308628d4c205d60898
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968098"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = new TokenIssuancePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenIssuancePolicy.definition = definitionList;
tokenIssuancePolicy.displayName = "displayName-value";
tokenIssuancePolicy.isOrganizationDefault = true;

graphClient.policies().tokenIssuancePolicies()
    .buildRequest()
    .post(tokenIssuancePolicy);

```