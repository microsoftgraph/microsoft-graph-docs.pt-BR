---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03556b111e8036e5ec85c776c65ee68e9f94800f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224494"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedValue = new AllowedValue
{
    Id = "Alpine",
    IsActive = true
};

await graphClient.Directory.CustomSecurityAttributeDefinitions["{customSecurityAttributeDefinition-id}"].AllowedValues
    .Request()
    .AddAsync(allowedValue);

```