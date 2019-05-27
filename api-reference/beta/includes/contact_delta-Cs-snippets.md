---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebb9821aaa5520ff215d02481ac1c66f629beb4b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders["{id}"].Contacts.Delta()
    .Request()
    .Select( e => new {
             e.DisplayName 
             })
    .GetAsync();

```