---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11e41490096e441a64cffcb98e9c3579344a5de6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508731"
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