---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa20152636e355eef659915b7c9480596dd469f2f4b66717a5ac1aa944ca3ffe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("includeHiddenFolders", "true")
};

var mailFolders = await graphClient.Me.MailFolders
    .Request( queryOptions )
    .GetAsync();

```