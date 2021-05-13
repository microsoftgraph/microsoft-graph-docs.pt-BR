---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8aa95f391ac61cbaf09369c309124878b6531dd8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475300"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleCollectionPage roleEligibilitySchedules = graphClient.roleManagement().directory().roleEligibilitySchedules()
    .buildRequest()
    .get();

```