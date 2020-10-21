---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9702795737d7b370ed8999458513e984e0384904
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Me.Drive
    .Request()
    .GetAsync();

```