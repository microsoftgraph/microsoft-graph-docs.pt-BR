---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba5f6b32ee03552f78957d950f0182639366663d64ec3c6f23d86fe339c4aff2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columns = await graphClient.Sites["{site-id}"].Columns
    .Request()
    .GetAsync();

```