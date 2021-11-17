---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a644442d3dbfb09efb01c37c4b99dcaf10154b872638aced7d04af689aaade6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bitlockerRecoveryKey = await graphClient.InformationProtection.Bitlocker.RecoveryKeys["{bitlockerRecoveryKey-id}"]
    .Request()
    .Select("key")
    .GetAsync();

```