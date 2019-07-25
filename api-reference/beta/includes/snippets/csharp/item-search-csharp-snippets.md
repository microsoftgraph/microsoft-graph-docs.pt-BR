---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04584112fda822b38f030ea017a88372cf1c421d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search('{search-query}')
    .Request()
    .GetAsync();

```