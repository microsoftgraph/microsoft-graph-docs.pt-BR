---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f42370830f016c23454704d35c02dbad884b87c0e1d51361bacd3a7402ca2642
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100188"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var passwordMethods = await graphClient.Me.Authentication.PasswordMethods
    .Request()
    .GetAsync();

```