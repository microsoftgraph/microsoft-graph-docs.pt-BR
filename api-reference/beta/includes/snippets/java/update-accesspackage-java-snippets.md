---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 009d5a93a149092b1a96227908ada11f696da499
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952253"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackage accessPackage = new AccessPackage();
accessPackage.displayName = "Access Package New Name";

graphClient.identityGovernance().entitlementManagement().accessPackages("{accessPackageId}")
    .buildRequest()
    .patch(accessPackage);

```