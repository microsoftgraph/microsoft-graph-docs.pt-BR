---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2059e55c3c7a3337b4f75461506282f660728be
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507361"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var categories = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Categories
    .Request()
    .GetAsync();

```