---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e44a8065f084e430737d39580799c198dfbe8ead54ebf80e50ee877b126974c6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleDefinitions = await graphClient.RoleManagement.CloudPC.RoleDefinitions
    .Request()
    .GetAsync();

```