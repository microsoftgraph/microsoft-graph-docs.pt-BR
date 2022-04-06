---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f022887215497e1e955a3fdc596f68f15f4c8837
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758222"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Bundles["{driveItem-id}"].Children["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```