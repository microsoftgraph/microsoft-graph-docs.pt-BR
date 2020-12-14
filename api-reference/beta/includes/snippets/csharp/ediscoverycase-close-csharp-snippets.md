---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8005da71d27bd48c7c6a43d13f7c492b2dd11d4c
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657049"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["061b9a92-8926-4bd9-b41d-abf35edc7583"]
    .Close()
    .Request()
    .PostAsync();

```