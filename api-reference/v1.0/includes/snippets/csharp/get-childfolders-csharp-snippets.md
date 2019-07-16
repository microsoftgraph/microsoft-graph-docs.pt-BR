---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 225977cd90be1c813c8489792b21b01d95008e5b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var childFolders = await graphClient.Me.MailFolders["{id}"].ChildFolders
    .Request()
    .GetAsync();

```