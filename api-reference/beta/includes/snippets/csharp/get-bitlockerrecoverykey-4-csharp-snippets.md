---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0a6279c414a6b03e2c96c60ae4efd3c4b07bd18
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bitlockerRecoveryKey = await graphClient.InformationProtection.Bitlocker.RecoveryKeys["{bitlockerRecoveryKey-id}"]
    .Request()
    .Select("key")
    .GetAsync();

```