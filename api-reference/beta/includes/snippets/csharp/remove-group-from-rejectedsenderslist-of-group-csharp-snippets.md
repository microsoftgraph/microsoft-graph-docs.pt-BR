---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c42788da852c26976d2c06e2091fe9ff8cf94a44
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "35858831"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].RejectedSenders.References
    .Request()
    .DeleteAsync();

```