---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89f54da44b41c23e06f84e325ef5cc89d9b2f279
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicyCollectionPage assignmentPolicies = graphClient.identityGovernance().entitlementManagement().assignmentPolicies()
    .buildRequest()
    .get();

```