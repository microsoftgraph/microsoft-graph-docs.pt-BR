---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8395d7d42c9636d18f517679436f63d7ee8c8d16
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35721466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Request()
    .DeleteAsync();

```