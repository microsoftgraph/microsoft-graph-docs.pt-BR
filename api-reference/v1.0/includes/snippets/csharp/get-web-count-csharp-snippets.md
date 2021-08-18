---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5fc2d1d55eaf04fdf909093830bf716f084ab9e4fa39cfe0ccdca3e21c862afe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Web")
    .GetAsync();

```