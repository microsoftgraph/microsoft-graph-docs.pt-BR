---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 731d2eed800b134c9ca598be8760f0afbb64c73f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{id|userPrincipalName}"].Manager
    .Request()
    .GetAsync();

```