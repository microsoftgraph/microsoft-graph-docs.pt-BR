---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbd6586b0cedcbd98e637f64b605fbf63b900997
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890048"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getYammerGroupsActivityGroupCounts('D7')
    .buildRequest()
    .get();

```