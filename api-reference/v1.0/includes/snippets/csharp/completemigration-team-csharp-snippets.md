---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4109ce0191ae5791492aa9ab713b921032a92f9e0a7e9e94fc079619a0817b79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```