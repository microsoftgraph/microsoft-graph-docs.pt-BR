---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9bfb9279250cf11e461108a6ea56a72977dcf8229adaf6357d7004e4ceac214
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898780"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = new AccessPackageAssignmentRequest();
accessPackageAssignmentRequest.requestType = "AdminRemove";
AccessPackageAssignment accessPackageAssignment = new AccessPackageAssignment();
accessPackageAssignment.id = "a6bb6942-3ae1-4259-9908-0133aaee9377";
accessPackageAssignmentRequest.accessPackageAssignment = accessPackageAssignment;

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .post(accessPackageAssignmentRequest);

```