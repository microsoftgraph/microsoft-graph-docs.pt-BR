---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 758dd04714770d13d46e9aa1248cc0052b05ba16a7d34cbb74e6eced2ef0f4d6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160187"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"].Rubric.Reference
    .Request()
    .PutAsync("{id}");

```