---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6f1a2651a6c7319c8f8cabe9c26511ede97d2ab
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .DeleteAsync();

```