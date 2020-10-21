---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0ac643ad2212bbbf56c55c89cf4f59f07e223623
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Groups["{groupId}"].Drives
    .Request()
    .GetAsync();

```