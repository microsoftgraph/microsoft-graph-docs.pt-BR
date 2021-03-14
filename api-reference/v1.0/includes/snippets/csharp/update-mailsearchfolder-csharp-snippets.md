---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65ac6dbe9161df302b326de2a4f19e97e8269621
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = new MailSearchFolder
{
    FilterQuery = "contains(subject, 'Analytics')"
};

await graphClient.Me.MailFolders["{mailFolder-id}"]
    .Request()
    .UpdateAsync(mailFolder);

```