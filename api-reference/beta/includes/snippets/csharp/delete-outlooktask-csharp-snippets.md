---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 830833e744687229273dbb876a9ea5bb122f9e9c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.Tasks["{outlookTask-id}"]
    .Request()
    .DeleteAsync();

```