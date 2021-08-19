---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc521d10802ad49df543b770c9b983e2c426360959ea29d923cbd4830180f2ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric
    .Request()
    .GetAsync();

```