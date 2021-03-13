---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1918ffb11b8e2ddfcb5906c496c151746d1ceafb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignment = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Request()
    .GetAsync();

```