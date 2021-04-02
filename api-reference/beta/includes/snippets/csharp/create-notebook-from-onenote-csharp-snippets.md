---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 756ff7e43e59ca811f93b0e675aa8250c1e88dfb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = new Notebook
{
    DisplayName = "My Private notebook"
};

await graphClient.Me.Onenote.Notebooks
    .Request()
    .AddAsync(notebook);

```