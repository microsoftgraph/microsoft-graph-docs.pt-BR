---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84a21f48e0315273e3c157fabad304b05ee486a4
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34546569"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new Attachment
{
    Name = "name-value",
    Item = "message or event entity"
};

await graphClient.Me.Events["{id}"].Attachments
    .Request()
    .AddAsync(attachment);

```