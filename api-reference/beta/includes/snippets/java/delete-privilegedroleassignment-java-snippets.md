---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2aa8e4e70d6da910a894798f3d9bbfc06b1910a0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875766"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.privilegedRoleAssignments("{id}")
    .buildRequest()
    .delete();

```