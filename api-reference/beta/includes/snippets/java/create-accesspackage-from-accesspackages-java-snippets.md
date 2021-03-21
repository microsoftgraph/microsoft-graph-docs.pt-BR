---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31aaa3330322586056590c75f49b8bf38eeb52e9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.catalogId = "aa2f6514-3232-46e7-a08a-2411ad8d7128";
accessPackage.displayName = "sales reps";
accessPackage.description = "outside sales representatives";

graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .post(accessPackage);

```