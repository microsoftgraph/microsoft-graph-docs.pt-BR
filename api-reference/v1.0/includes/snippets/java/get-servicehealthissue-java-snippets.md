---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09ed2decdd2eb58f20caf815361551f5e01e2c39
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265924"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthIssue serviceHealthIssue = graphClient.admin().serviceAnnouncement().issues("MO226784")
    .buildRequest()
    .get();

```