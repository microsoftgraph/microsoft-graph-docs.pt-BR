---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67de6ae1cec241c772b8fa0806fd54f39062f1a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Publications["{itemPublication-id}"]
    .Request()
    .DeleteAsync();

```