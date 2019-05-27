---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 564a460f582775cbd86de53be9379281ed7ebdbe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Me.Contacts
    .Request()
    .Select( e => new {
             e.DisplayName,
             e.EmailAddresses 
             })
    .GetAsync();

```