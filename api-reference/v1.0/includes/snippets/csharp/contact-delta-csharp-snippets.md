---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88cd1ac7a6b53184806ca1b719610d632be92cc2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{id}"].Contacts
    .Delta()
    .Request()
    .Header("Prefer","odata.maxpagesize=2")
    .Select( e => new {
             e.DisplayName 
             })
    .GetAsync();

```