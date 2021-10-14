---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9bd2cbb2ec5149767cebb3b00f03af0c31c1f7a59e8572f9789cc403e8e4bf9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Contacts["{orgContact-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```