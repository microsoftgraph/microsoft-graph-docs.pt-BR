---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9b979832c4cc7a07c555fefff66ba11d741dffb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758086"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Items["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```