---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c42788da852c26976d2c06e2091fe9ff8cf94a44
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].RejectedSenders.References
    .Request()
    .DeleteAsync();

```