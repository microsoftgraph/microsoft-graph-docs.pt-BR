---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12ec01f1f30c21056665b9c67bed98f41127cf0f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955517"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskDetection = await graphClient.IdentityProtection.RiskDetections["{riskDetection-id}"]
    .Request()
    .GetAsync();

```