---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73c341e02fb6630f9190078cb6504e3f447d7e30e8051b973fbb6fdfa4908ace
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRole = await graphClient.DirectoryRoles["{directoryRole-id}"]
    .Request()
    .GetAsync();

```