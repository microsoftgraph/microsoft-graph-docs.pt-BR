---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53170526cf8508a7e21599a0b58c13a370277f2d0e74134d0cd6b1c3986d17d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Classes["{educationClass-id}"].Assignments["{educationAssignment-id}"]
    .SetUpResourcesFolder()
    .Request()
    .PostAsync();

```