---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa8bc94e1c9e999ed1581507d9a80b94f522e079
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111051"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Users["{educationUser-id}"].Assignments
    .Request()
    .GetAsync();

```