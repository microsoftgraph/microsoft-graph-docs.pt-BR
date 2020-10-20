---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b7d1a86d56b923d0e951c5ca00dfc6e21e4844c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619635"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = false;

await graphClient.Groups["{id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```