---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 36e747212698ce881d05304263180d9b18506e62
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967497"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentResourceRole accessPackageAssignmentResourceRole = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles("{id}")
    .buildRequest()
    .get();

```