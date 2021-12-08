---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 424108addcb7338263d6cef4bef56d72d07101af
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCollectionPage accessPackages = graphClient.identityGovernance().entitlementManagement().accessPackages()
    .buildRequest()
    .get();

```