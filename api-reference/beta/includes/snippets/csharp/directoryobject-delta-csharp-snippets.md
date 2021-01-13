---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 475e22a11e419edc8124de72e111ec6288dc6ed1
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845964"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.DirectoryObjects["delta"]
    .Request()
    .Filter("isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')")
    .GetAsync();

```