---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91d32f32c51b4cb9c63f6f05e16f8cc94ee09391
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "04487ee0-f4f6-4e7f-8999-facc5a30e232"
};

await graphClient.IdentityProtection.RiskyUsers
    .Dismiss(userIds)
    .Request()
    .PostAsync();

```