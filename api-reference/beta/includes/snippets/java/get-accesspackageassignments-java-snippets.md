---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0fcc863294f73e5768124b396b0311ad11ce37c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageAssignmentCollectionPage accessPackageAssignments = graphClient.identityGovernance().entitlementManagement().accessPackageAssignments()
    .buildRequest()
    .get();

```