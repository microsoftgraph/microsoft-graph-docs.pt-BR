---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d30aa90532f0dd7b3aba987b66d90d4da150003c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603722"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threads = await graphClient.Groups["{id}"].Threads
    .Request()
    .GetAsync();

```