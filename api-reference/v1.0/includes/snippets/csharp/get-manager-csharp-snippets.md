---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 731d2eed800b134c9ca598be8760f0afbb64c73f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738460"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{id|userPrincipalName}"].Manager
    .Request()
    .GetAsync();

```