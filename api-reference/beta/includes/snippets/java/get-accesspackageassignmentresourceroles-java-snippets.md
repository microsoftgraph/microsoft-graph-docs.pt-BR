---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 126f3bcfeda7c379e7127be5ff799f6457bea544
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952001"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageAssignmentResourceRoleCollectionPage accessPackageAssignmentResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles()
    .buildRequest()
    .get();

```