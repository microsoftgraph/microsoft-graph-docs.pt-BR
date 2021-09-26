---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 911e2a3d6721323229bc033075fc5b75413b666a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765673"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Device device = graphClient.devices("000005c3-b7a6-4c61-89fc-80bf5ccfc366")
    .buildRequest()
    .get();

```