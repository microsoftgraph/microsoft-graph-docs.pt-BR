---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa63b98f3a7ab441a911d8bf69ac7a59bd44fef1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332772"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Filter("hasMembersWithLicenseErrors+eq+true,")
    .Select( e => new {
             e.Id,
             e.DisplayName 
             })
    .GetAsync();

```