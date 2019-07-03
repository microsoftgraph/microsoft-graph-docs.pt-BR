---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24d3b28bb12c00f65ab44d6ead523e069a16a496
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetections = await graphClient.RiskDetections
    .Request()
    .Filter("riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .GetAsync();

```