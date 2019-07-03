---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfda948bf615e89610f1d1db5ed2daf54ed5cacc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook.SupportedTimeZones(microsoft.graph.timeZoneStandard'Iana')
    .Request()
    .GetAsync();

```