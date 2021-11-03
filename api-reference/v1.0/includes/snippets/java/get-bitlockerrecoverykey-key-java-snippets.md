---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eafca69cd7cc3051b0f306b05cdd204023de924a
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729882"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BitlockerRecoveryKey bitlockerRecoveryKey = graphClient.informationProtection().bitlocker().recoveryKeys("b465e4e8-e4e8-b465-e8e4-65b4e8e465b4")
    .buildRequest()
    .select("key")
    .get();

```