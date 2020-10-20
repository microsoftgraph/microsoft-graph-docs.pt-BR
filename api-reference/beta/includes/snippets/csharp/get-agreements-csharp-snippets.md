---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81cb511d07cb9f8079cc625eb4aab928c0ff0c6e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreements = await graphClient.Agreements
    .Request()
    .GetAsync();

```