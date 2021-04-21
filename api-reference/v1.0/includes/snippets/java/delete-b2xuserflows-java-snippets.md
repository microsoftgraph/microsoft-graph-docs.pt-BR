---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac012075fb7e5a447e85affd6945a090f14105c4
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner")
    .buildRequest()
    .delete();

```