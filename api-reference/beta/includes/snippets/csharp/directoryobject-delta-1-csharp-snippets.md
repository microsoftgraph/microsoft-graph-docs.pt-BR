---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68e4c5c425006f0446fddc45b8de7bd3af254f5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946626"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["{directoryObject-id}"]
    .Request()
    .Header("Prefer","return=minimal")
    .GetAsync();

```