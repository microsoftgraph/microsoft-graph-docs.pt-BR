---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 503eaeaaa490e02596e57c4dfb3bfb12137e4c29
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342843"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequestCollectionPage assignmentRequests = graphClient.identityGovernance().entitlementManagement().assignmentRequests()
    .buildRequest()
    .get();

```