---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8966cc8cff64e7e98537747be28a760e40df5ea1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityActions = await graphClient.Security.SecurityActions
    .Request()
    .GetAsync();

```