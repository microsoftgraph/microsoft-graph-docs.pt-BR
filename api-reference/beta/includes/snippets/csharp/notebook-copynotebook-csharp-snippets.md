---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9be007f0a702a63e5cf797f6da614590c32f8a67
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781465"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Notebooks["{notebook-id}"]
    .CopyNotebook(groupId,renameAs,null,null,null)
    .Request()
    .PostAsync();

```