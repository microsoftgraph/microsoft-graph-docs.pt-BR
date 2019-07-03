---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33a360bc41eafde3315a28142ee02bc776fbb29
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476038"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groups = await graphClient.Groups
    .Request()
    .Filter("hasMembersWithLicenseErrors+eq+true,")
    .Select( e => new {
             e.Id,
             e.DisplayName 
             })
    .GetAsync();

```