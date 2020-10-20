---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f93ebfc3c12d0b88fa77b53fe1eeeee2a94a3191
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619273"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Contacts["{id}"]
    .Request()
    .DeleteAsync();

```