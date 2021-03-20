---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3dea140aae6b545b4197cfcc94dbf93146f3302
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978849"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "HiddenMembership";

graphClient.administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```