---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 281ce9103615bb3e696e6f464155654cd4bca6bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationAssignmentDefaults = await graphClient.Education.Classes["{educationClass-id}"].AssignmentDefaults
    .Request()
    .GetAsync();

```