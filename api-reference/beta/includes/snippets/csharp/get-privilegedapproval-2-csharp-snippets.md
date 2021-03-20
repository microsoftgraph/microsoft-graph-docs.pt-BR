---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7256b6fab723f80774692c49c814fe9a74bf146f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedApproval = await graphClient.PrivilegedApproval
    .Request()
    .GetAsync();

```