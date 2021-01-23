---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70abb45ba907021eb753154508dbfa11b917fefa
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connector = await graphClient.OnPremisesPublishingProfiles["applicationProxy"].Connectors["{id}"]
    .Request()
    .GetAsync();

```