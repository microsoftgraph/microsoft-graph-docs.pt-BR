---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb8fbd3e51cdea9bab0bba3c293542920b4b1a14
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666463"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("includeHiddenFolders", "true")
};

var childFolders = await graphClient.Me.MailFolders["{mailFolder-id}"].ChildFolders
    .Request( queryOptions )
    .GetAsync();

```