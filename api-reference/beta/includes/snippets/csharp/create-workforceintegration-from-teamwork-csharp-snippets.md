---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a115e5007131dbe671856b9b2748112972bb3a1d2e9cfde6af5a96fb2acbd6a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegration = new WorkforceIntegration
{
    DisplayName = "displayName-value",
    ApiVersion = 99,
    Encryption = new WorkforceIntegrationEncryption
    {
        Protocol = WorkforceIntegrationEncryptionProtocol.SharedSecret,
        Secret = "secret-value"
    },
    IsActive = true,
    Url = "url-value",
    Supports = WorkforceIntegrationSupportedEntities.None
};

await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .AddAsync(workforceIntegration);

```