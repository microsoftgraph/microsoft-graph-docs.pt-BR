---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f338bad59cda1992448c456d9af89ec140d3cb17225a23a577932110bba09613
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160264"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenIssuancePolicy tokenIssuancePolicy = new TokenIssuancePolicy();
LinkedList<String> definitionList = new LinkedList<String>();
definitionList.add("definition-value");
tokenIssuancePolicy.definition = definitionList;
tokenIssuancePolicy.displayName = "displayName-value";
tokenIssuancePolicy.isOrganizationDefault = true;

graphClient.policies().tokenIssuancePolicies("{id}")
    .buildRequest()
    .patch(tokenIssuancePolicy);

```