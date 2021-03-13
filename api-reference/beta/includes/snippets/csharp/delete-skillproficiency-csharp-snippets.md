---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa9137545e6c008cbf7e4aa1c16ebcaf976702cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Skills["{skillProficiency-id}"]
    .Request()
    .DeleteAsync();

```