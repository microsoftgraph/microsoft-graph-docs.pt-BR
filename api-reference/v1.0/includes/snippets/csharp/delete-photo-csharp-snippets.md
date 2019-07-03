---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62c6d0e7a1356efe68e04fa2867737c6da1cce53
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35465630"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{id|userPrincipalName}"].Photo
    .Request()
    .DeleteAsync();

```