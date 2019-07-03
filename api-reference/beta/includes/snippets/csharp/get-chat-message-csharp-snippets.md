---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39b1c2db4bcf38c17f178e71a8ee0489e1d59a6b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477225"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = await graphClient.Users["{id}"].Chats["{id}"]
    .Request()
    .GetAsync();

```