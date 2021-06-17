---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48aedab16b265c5b0fc1ae59467e3ae49626c021
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990862"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.DirectoryRoles["{directoryRole-id}"].Members
    .Request()
    .GetAsync();

```