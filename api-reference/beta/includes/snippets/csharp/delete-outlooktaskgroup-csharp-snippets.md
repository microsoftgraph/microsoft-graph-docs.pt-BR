---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd67b380573b098aa8a95814212ff102b7b9f49c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Outlook.TaskGroups["{outlookTaskGroup-id}"]
    .Request()
    .DeleteAsync();

```