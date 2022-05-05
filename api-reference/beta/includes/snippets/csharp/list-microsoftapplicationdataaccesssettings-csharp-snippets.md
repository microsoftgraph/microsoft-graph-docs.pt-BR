---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f50e7f98dbc2c867f43a915e76d712dbfdd7e70
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftApplicationDataAccessSettings = await graphClient.Organization["{organization-id}"].Settings.MicrosoftApplicationDataAccess
    .Request()
    .GetAsync();

```