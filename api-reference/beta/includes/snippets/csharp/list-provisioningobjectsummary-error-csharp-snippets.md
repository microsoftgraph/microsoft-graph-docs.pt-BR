---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee81ca41dd4a3eda52e5868b52cb33e0c9b4f16e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723375"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var provisioning = await graphClient.AuditLogs.Provisioning
    .Request()
    .GetAsync();

```