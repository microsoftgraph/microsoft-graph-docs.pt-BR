---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3c775c40d8e18f27ccc8510d51e01d5b37952360
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855859"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .delete();

```