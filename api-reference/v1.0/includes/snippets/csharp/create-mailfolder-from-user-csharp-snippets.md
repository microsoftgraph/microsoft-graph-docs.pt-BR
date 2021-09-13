---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6b349934fa69f1c4b3c24cd745ad6121cd731d91d8f397771f662ac4c635694
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897969"
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