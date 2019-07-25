---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2632754f847180622a45953fb9ca68dbfbfc686
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875858"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRole privilegedRole = graphClient.privilegedRoles("{id}")
    .buildRequest()
    .get();

```