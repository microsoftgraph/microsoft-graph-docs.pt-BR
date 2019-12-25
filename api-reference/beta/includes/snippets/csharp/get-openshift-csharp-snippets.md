---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44f196c8bab591c77b98bbcd949386116a2faaf5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShifts = await graphClient.Teams["{id}"].Schedule.OpenShifts
    .Request()
    .GetAsync();

```