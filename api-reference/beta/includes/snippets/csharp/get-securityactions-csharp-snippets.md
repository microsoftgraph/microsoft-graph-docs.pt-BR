---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3fab943b1c72deb025fa009cb0b4362949fc275d12ec86de27afadde19538cb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272995"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityActions = await graphClient.Security.SecurityActions
    .Request()
    .GetAsync();

```