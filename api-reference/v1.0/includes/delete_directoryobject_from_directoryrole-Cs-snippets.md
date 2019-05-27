---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3b5c0c800d2ffc520322ca50da091f8ebffaa13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459304"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{id}"].Members["{id}"]
    .Request()
    .DeleteAsync();

```