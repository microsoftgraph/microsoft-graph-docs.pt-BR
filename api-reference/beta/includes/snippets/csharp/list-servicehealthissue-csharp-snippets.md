---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7c483cb66113dfed119ecf5d3bb18abe2f6a253
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208885"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var issues = await graphClient.Admin.ServiceAnnouncement.Issues
    .Request()
    .GetAsync();

```