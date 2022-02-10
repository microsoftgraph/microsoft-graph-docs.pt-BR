---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b455534facfc80fdcc51a6a2418e6c49b81d3975
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519279"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Tasks.Lists["{baseTaskList-id}"]
    .Request()
    .DeleteAsync();

```