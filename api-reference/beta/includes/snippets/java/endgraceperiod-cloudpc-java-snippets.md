---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70ad4f1e11b17b8e2c0fbd8dbafe96543910f4c3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59765877"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().cloudPCs("{cloudPCId}")
    .endGracePeriod()
    .buildRequest()
    .post();

```