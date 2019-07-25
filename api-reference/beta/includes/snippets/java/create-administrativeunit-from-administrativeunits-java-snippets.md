---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4ef49dd84cf7e72eafaeb1dce920fae6dae6eff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855746"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "true";

graphClient.administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```