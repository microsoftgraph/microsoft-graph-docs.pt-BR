---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd353ed8bd8247b773c46e65b5d58ca8fc604cfc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["{directoryRole-id}"]
    .Request()
    .GetAsync();

```