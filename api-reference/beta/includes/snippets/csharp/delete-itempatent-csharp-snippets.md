---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2676ce158317a757edfc22140c5af4133aa844e3bde7fd9ded9f41e67f29d121
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Profile.Patents["{itemPatent-id}"]
    .Request()
    .DeleteAsync();

```