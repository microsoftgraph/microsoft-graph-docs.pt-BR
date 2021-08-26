---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 192c250f1eb42872300d11045d995d3b68fbe70eaaf1fb9595dd8941c6598508
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274565"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = new Device();
device.accountEnabled = false;

graphClient.devices("{id}")
    .buildRequest()
    .patch(device);

```