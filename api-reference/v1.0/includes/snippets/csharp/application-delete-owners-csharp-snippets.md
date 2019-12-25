---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f65531bc927dff1b27aa2a2284d697445fb45464
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Applications["{id}"].Owners["{id}"].Reference
    .Request()
    .DeleteAsync();

```