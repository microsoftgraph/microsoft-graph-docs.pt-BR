---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eca32b1aa75a09c03d3803a8f325ffe3c9594543
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37402414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("identities/any(c:c/issuerAssignedId eq 'j.smith@yahoo.com' and c/issuer eq 'contoso.onmicrosoft.com')")
    .Select( e => new {
             e.DisplayName,
             e.Id 
             })
    .GetAsync();

```