---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df1318ac364de0cdb5a348d5efa2690bf484c274
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976307"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentResourceRoleCollectionPage accessPackageAssignmentResourceRoles = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentResourceRoles()
    .buildRequest()
    .get();

```