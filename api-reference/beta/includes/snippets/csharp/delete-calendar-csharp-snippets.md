---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 168d963ab77e81f46725e5846653c8be2c6e8a12
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615607"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Calendar
    .Request()
    .DeleteAsync();

```