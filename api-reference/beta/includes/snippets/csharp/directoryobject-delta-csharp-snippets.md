---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd9e920f849acb8299eb59db38d24b66e59e555b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706778"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User')+or+isOf('Microsoft.Graph.Group')")
    .GetAsync();

```