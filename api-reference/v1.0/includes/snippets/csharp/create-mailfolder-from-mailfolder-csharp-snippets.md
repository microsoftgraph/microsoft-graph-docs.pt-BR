---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ed3ddeeb4312d7cfe3ce04517a635ab9282abd31c913bbb50cdaa0a488c8b76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275306"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailFolder
{
    DisplayName = "displayName-value",
    IsHidden = true
};

await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request()
    .AddAsync(mailFolder);

```