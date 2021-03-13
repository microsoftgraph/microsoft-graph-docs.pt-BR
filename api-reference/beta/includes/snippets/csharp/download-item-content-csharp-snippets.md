---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63112b7be88ea7834c90568fd527d4a0e573509a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request()
    .GetAsync();

```