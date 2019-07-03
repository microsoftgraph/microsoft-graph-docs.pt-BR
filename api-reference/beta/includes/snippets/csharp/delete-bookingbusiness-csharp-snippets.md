---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6f1a2651a6c7319c8f8cabe9c26511ede97d2ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463258"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.BookingBusinesses["fabrikam@M365B489948.onmicrosoft.com"]
    .Request()
    .DeleteAsync();

```