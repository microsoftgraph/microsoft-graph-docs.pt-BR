---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7be05ffd1451446b5ecb56e921b4bf49e81f0f18
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684726"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Filter("startswith(displayName,'Eric'),")
    .Select("displayName,signInActivity")
    .GetAsync();

```