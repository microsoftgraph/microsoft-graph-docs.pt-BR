---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96c123debdda567bfc200b30d65b3c9a9bce6cef
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996307"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.UserPrincipalName 
             })
    .GetAsync();

```