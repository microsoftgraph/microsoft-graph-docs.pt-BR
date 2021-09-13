---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 729b8e5d4caa1b36258060c710f801e53e70ed4d7a01ca5eb91bfb77cecbd23c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = new FileAttachment
{
    Name = "smile",
    ContentBytes = Encoding.ASCII.GetBytes("R0lGODdhEAYEAA7")
};

await graphClient.Me.Messages["{message-id}"].Attachments
    .Request()
    .AddAsync(attachment);

```