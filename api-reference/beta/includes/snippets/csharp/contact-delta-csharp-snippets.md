---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ebb9821aaa5520ff215d02481ac1c66f629beb4b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517681"
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