---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54b104649dc0caa53412b07f321a009d45a3ef6c
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "Clutter",
    IsHidden = true
};

await graphClient.Me.MailFolders
    .Request()
    .AddAsync(mailFolder);

```