---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d6b76496572f903bacf2a00d1154c26ca9b7c0b
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentSchedule unifiedRoleAssignmentSchedule = graphClient.roleManagement().directory().roleAssignmentSchedules("226faf5f-61b4-40bb-8726-52e48ec914de")
    .buildRequest()
    .get();

```