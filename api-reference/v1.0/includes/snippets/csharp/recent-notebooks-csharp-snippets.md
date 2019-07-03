---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68490dbb5aa9c5617abd8b36f05db8c580e2c9c7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRecentNotebooks = await graphClient.Me.Onenote.Notebooks.GetRecentNotebooks(true)
    .Request()
    .GetAsync();

```