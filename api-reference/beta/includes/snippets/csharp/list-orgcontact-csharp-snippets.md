---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 235b7a0e8a8fa24c2dcc19fe790f44b7a4292abe
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607819"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contacts = await graphClient.Contacts
    .Request()
    .GetAsync();

```