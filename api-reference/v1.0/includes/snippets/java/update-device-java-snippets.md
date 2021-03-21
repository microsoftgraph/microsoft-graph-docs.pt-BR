---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1df5b8b40e15ab16d9919f7301aa714aef49c13
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974020"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;

graphClient.devices("{id}")
    .buildRequest()
    .patch(device);

```