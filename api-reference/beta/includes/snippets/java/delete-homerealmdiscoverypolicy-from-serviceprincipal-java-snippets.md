---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7361e3c691ca5844ad840f5dd77197105a20b35f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969656"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{servicePrincipalId}").homeRealmDiscoveryPolicies("{policyId}").reference()
    .buildRequest()
    .delete();

```