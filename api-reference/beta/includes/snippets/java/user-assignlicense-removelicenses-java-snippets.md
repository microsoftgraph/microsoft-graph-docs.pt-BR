---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b92044d3ecd52d4044fedd30b4ace858c7f1101e
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339984"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<AssignedLicense> addLicensesList = new LinkedList<AssignedLicense>();

LinkedList<UUID> removeLicensesList = new LinkedList<UUID>();
removeLicensesList.add(UUID.fromString("f30db892-07e9-47e9-837c-80727f46fd3d"));
removeLicensesList.add(UUID.fromString("84a661c4-e949-4bd2-a560-ed7766fcaf2b"));

graphClient.me()
    .assignLicense(UserAssignLicenseParameterSet
        .newBuilder()
        .withAddLicenses(addLicensesList)
        .withRemoveLicenses(removeLicensesList)
        .build())
    .buildRequest()
    .post();

```