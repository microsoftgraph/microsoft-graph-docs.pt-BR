---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30e11ddf09fae50f5dc792eb1b4f99553e0e60241a6d06db6ad67d5e468bfec4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "alexd@contoso.com"
};

await graphClient.Groups["{group-id}"].RejectedSenders.References
    .Request()
    .AddAsync(directoryObject);

```