---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59a6542032b26b39388fe07078838082265eec26
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223068"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["contosohr"].Groups["31bea3d537902000"].Members["14m1b9c38qe647f6a"]
    .Request()
    .DeleteAsync();

```