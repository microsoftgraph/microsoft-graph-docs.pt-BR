---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93ce8a44569ca6bff742900572eb9b3e99b28ff2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614282"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfiles = await graphClient.Security.SecureScoreControlProfiles
    .Request()
    .GetAsync();

```