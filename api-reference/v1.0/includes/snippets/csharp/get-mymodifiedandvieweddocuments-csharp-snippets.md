---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ebaf7c50dcef76d77ce75d67051238f1fbce191
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var used = await graphClient.Me.Insights.Used
    .Request()
    .OrderBy("LastUsed/LastAccessedDateTime")
    .GetAsync();

```