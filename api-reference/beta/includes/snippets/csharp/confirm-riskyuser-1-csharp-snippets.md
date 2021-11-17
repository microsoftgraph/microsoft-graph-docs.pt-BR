---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 429d18391e1e2d5900cddfdd832a54dbd5d459fa4f6f7e3d618f851850a18d38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157063"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userIds = new List<String>()
{
    "29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
    "20f91ec9-d140-4d90-9cd9-f618587a1471"
};

await graphClient.RiskyUsers
    .ConfirmCompromised(userIds)
    .Request()
    .PostAsync();

```