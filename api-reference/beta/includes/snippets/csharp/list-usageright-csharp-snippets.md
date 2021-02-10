---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b4ca30c9aeebab2967357c2acffdc24a101fc8c
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179197"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var usageRights = await graphClient.Devices["{objectId}"].UsageRights
    .Request()
    .Filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .GetAsync();

```