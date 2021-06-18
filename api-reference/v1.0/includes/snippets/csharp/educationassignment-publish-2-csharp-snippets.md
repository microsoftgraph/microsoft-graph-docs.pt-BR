---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c07c0f75dcd5e6aeeb537e3262ce0e940e929285
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .Publish()
    .Request()
    .PostAsync();

```