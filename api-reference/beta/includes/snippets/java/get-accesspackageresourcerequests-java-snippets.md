---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b4893f5b2b1b8ece737d02721ab906f7a3283a1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977594"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageResourceRequestCollectionPage accessPackageResourceRequests = graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .get();

```