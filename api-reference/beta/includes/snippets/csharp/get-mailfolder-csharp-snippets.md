---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8515e2ae1bd170a18e5375c6bba60d97a7754e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mailFolder = await graphClient.Me.MailFolders["AAMkAGVmMDEzM"]
    .Request()
    .GetAsync();

```