---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca5299f7cf1bcd4a184ef9d132ca2655eeb8f9fb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209893"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = graphClient.identityGovernance().entitlementManagement().assignmentPolicies("{accessPackageAssignmentPolicyId}")
    .buildRequest()
    .get();

```