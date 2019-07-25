---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85b9278738196710f4408e9129b34ab126c9dcbc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.ContactFolders
    .Delta()
    .Request()
    .GetAsync();

```