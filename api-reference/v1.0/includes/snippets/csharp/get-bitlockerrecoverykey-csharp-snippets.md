---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a088a1a69596a35fb5f442f8dd6beda580c7bb4
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729854"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bitlockerRecoveryKey = await graphClient.InformationProtection.Bitlocker.RecoveryKeys["{bitlockerRecoveryKey-id}"]
    .Request()
    .Header("ocp-client-name","\"My Friendly Client\"")
    .Header("ocp-client-version","\"1.2\"")
    .GetAsync();

```