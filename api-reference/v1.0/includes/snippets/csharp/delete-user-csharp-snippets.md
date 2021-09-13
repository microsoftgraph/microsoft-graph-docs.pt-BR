---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6c02f3e93d009c76c6ea8db12b53c35e50e14ded3386ef49cc731f6ed6fe60e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"]
    .Request()
    .DeleteAsync();

```