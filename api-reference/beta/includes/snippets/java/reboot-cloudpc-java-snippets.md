---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44ac30a31e53b34d6f0a787b4f5505afccd60696
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524426"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().cloudPCs("831dd62e-cfa1-4d49-a3b4-58d4e9920f8e")
    .reboot()
    .buildRequest()
    .post();

```