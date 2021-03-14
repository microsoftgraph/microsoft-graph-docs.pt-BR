---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c65ade435b6d1bd5f16c7a9731d7798ef11e1678
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"]
    .Request()
    .DeleteAsync();

```