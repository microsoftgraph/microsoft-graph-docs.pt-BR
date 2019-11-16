---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f65531bc927dff1b27aa2a2284d697445fb45464
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37999072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```