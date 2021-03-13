---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 794f8e1e12414a561183b649c423e213b90f1d43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792316"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["{externalConnection-id}"]
    .Request()
    .DeleteAsync();

```