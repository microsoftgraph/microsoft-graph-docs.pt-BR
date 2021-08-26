---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30e4346dea26479d0a4d1ccd9b1fa829202fd6d96c01d869a65461b36cdaf807
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AccountEnabled = true,
    AlternativeSecurityIds = new List<AlternativeSecurityId>()
    {
        new AlternativeSecurityId
        {
            Type = 99,
            IdentityProvider = "identityProvider-value",
            Key = Encoding.ASCII.GetBytes("base64Y3YxN2E1MWFlYw==")
        }
    },
    ApproximateLastSignInDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    DeviceId = "deviceId-value",
    DeviceMetadata = "deviceMetadata-value",
    DeviceVersion = 99
};

await graphClient.Devices
    .Request()
    .AddAsync(device);

```