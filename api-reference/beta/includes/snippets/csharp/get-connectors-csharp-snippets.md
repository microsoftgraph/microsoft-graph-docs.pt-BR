---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44059049e842b5e3abd7f0a4264692db3fa33dd2
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50035788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].Connectors
    .Request()
    .GetAsync();

```