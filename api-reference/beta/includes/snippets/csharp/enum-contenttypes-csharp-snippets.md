---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1d5ec95c5e3926cea897cf7cc64493ec2e0f2ef1e5fcd7d84f13c7c17fd2d2cf
ms.sourcegitcommit: 24d0ea8e2bcb54c2f397133460c3d26fb0ba705f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2021
ms.locfileid: "60730008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypes = await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .Request()
    .GetAsync();

```