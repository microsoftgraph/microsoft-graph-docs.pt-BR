---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8056d8ab09234c37b4d13c762447cb2a3e072d4a6368c6bfdd675518dd9d19a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213604"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "Display name"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```