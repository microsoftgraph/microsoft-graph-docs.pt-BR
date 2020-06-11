---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8014fa97b12838370e9716c4efee1ca5e3089f6
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Users
    .Request()
    .Select("displayName,givenName,postalCode")
    .GetAsync();

```