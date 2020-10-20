---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11e41490096e441a64cffcb98e9c3579344a5de6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612872"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = new Notebook
{
    DisplayName = "Notebook name"
};

await graphClient.Me.Onenote.Notebooks
    .Request()
    .AddAsync(notebook);

```