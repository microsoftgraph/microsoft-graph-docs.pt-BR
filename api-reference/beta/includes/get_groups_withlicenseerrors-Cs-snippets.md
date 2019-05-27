---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b33a360bc41eafde3315a28142ee02bc776fbb29
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449493"
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