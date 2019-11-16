---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1cd9bcc652659b1e8ba2bdd3b3ef61baf6e6b5f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "35733750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.GivenName,
             e.PostalCode 
             })
    .GetAsync();

```