---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: baa5601ad084bc637b3bd5aced09fe99e9d849a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{educationSchool-id}"].Classes["{educationClass-id}"]
    .Request()
    .DeleteAsync();

```