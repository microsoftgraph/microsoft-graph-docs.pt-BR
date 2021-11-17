---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9c7f254848fb89ea2334ca1a6713f3bdb710efa0a0eab363bb704d7b083e669
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099717"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordCredential = new PasswordCredential
{
    DisplayName = "Password friendly name"
};

await graphClient.Applications["{application-id}"]
    .AddPassword(passwordCredential)
    .Request()
    .PostAsync();

```