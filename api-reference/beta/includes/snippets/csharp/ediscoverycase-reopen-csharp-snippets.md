---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 875178d0fa3c3223bc28df32445792d14598748b
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657059"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["061b9a92-8926-4bd9-b41d-abf35edc7583"]
    .Reopen()
    .Request()
    .PostAsync();

```