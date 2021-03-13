---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c21d2f56ed87f93b231edb555fb156099b659878
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796391"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .GetAsync();

```