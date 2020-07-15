---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44059049e842b5e3abd7f0a4264692db3fa33dd2
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142315"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].Connectors
    .Request()
    .GetAsync();

```