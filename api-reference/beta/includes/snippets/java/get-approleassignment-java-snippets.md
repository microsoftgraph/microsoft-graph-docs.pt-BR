---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb93e5c41be38c7bd54ce0dbad42e4891825c4ec
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppRoleAssignment appRoleAssignment = graphClient.appRoleAssignments("{id}")
    .buildRequest()
    .get();

```