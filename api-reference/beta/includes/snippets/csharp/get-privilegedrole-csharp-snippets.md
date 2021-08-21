---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8548b26d06848075cf7d63a2d9f7401543d1d6ba24754ef2b1f303636370134e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRole = await graphClient.PrivilegedRoles["{privilegedRole-id}"]
    .Request()
    .GetAsync();

```