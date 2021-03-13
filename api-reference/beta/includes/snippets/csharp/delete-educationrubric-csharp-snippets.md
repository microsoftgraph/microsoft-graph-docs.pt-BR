---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 046a6eac5f6ea4387178add9838813c1dcf1da81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802810"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .DeleteAsync();

```