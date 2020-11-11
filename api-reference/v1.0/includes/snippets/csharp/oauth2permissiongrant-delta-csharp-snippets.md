---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aac91df27735db5f8a9bbe6114720f748d0f8444
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Oauth2PermissionGrants
    .Delta()
    .Request()
    .GetAsync();

```