---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 799852a1b08cd00a9ae85c554670fdb4a5ef2cbc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{educationUser-id}"]
    .Request()
    .GetAsync();

```