---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1cd9bcc652659b1e8ba2bdd3b3ef61baf6e6b5f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
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